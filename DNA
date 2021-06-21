import pandas as pd
import csv
import sys
import re

def main():

    # Ensure correct usage
    if len(sys.argv) != 3:
        sys.exit("Usage: python dna.py data.csv sequence.txt")

    # Read CSV file into pandas dataframe
    df1 = pd.read_csv(sys.argv[1], header=0, index_col=0)

    # Read DNA sequence
    with open(sys.argv[2], "r") as f:
        DNA_sequence = f.read()

    # Create a dictionary where each column name is a STR
    # and its value is the longest number of repetitions
    dic = {}
    for i in range(len(df1.columns)):
        dic[df1.columns[i]] = [repeats(DNA_sequence, df1.columns[i])]

    # Convert dictionary to dataframe
    df2 = pd.DataFrame.from_dict(dic)

    # Concatenate the two dataframe putting df2 at the bottom
    mm = pd.concat([df1, df2], verify_integrity=True)

    # Subtract each row from the bottom row, if difference is zero: print match!
    for i in range(len(mm.iloc[:-1, 0])):
        diff = sum(mm.iloc[-1] - mm.iloc[i])

        if diff == 0:
            print(mm.index[i])
            sys.exit()

    # If we dont find a DNA match
    print("No match")


def repeats(sequence, STR):

    # Using max() + re.findall() to find the longest consecutive substring
    # Using count() to count the number of occurence
    count = max(re.findall('((?:' + re.escape(STR) + ')*)', sequence), key=len).count(STR)

    return count


main()
