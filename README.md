# Touch-stroke-dictionary-attack

The first block of the code is just calling all the required packages (libraries).

read_dataset function:
This function reads the dataset.
Drops "document ID" and "Phone ID" columns.
And looks for "NaN" values if there is any and drops those rows.

number_of_attackers function:
It gets three arguments: the first one is the predicted results, and the second on is the attackers dataset, and the third one is the threshold.
It just prints out the "user id" corresponding to the attackers who had at least a certain number of similarities which is definded by the threshold.

Finally, the main script:
First we read the dataset.
then for simplicity we set the threshold to 5, but it can be modified by the researcher (i.e., the threshold can vary according the researcher's preference).
The "for loop" in the implementation repeats the attacking process for all the 31 users.
The first step is to split the dataset into two parts: a training set and an attacking set.
Then, the classifiers are run and the results are printed.
