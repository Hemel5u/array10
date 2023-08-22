#!/bin/bash

# Initialize an empty array
words=()

echo "Please enter 10 words:"

# Loop to read 10 words from the user
for ((i=1; i<=10; i++)); do
    read -p "Word $i: " word
    words+=("$word")  # Add the word to the array
done

# Print the array elements
echo "The entered words are:"
for word in "${words[@]}"; do
    echo "$word"
done
