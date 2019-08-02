find the issues plz


##########################
# 6.00.2x Problem Set 1: Space Cows 

from ps1_partition import get_partitions
import time

#================================
# Part A: Transporting Space Cows
#================================

def load_cows('C:\Users\Joseph\Desktop\New folder (5)\PS1\ps1_cow_data.txt'):
    """
    Read the contents of the given file.  Assumes the file contents contain
    data in the form of comma-separated cow name, weight pairs, and return a
    dictionary containing cow names as keys and corresponding weights as values.
    Parameters:
    filename - the name of the data file as a string
    Returns:
    a dictionary of cow name (string), weight (int) pairs
    """

    cow_dict = dict()

    f = open('C:\Users\Joseph\Desktop\New folder (5)\PS1\ps1_cow_data.txt', 'r')
    
    for line in f:
        line_data = line.split(',')
        cow_dict[line_data[0]] = int(line_data[1])
    return cow_dict
