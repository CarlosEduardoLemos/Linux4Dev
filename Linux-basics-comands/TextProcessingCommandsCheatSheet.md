**Text Processing Commands Cheat Sheet - @csaba_kissi**

# 1. Search for a pattern in a file
```bash
grep 'pattern' filename
```

# 2. Search recursively for a pattern in all files in a directory
```bash
grep -r 'pattern' /path/to/directory
```

# 3. Replace text in a file using `sed`
```bash
sed 's/old_text/new_text/g' filename
```

# 4. Print lines 1 to 5 of a file
```bash
sed -n '1,5p' filename
```

# 5. Extract specific columns from a file (e.g., column 1 and 3)
```bash
cut -d ' ' -f 1,3 filename
```

# 6. Sort lines in a file alphabetically
```bash
sort filename
```

# 7. Remove duplicate lines from a sorted file
```bash
uniq filename
```

# 8. Count the number of lines, words, and characters in a file
```bash
wc filename
```

# 9. Convert lowercase to uppercase
```bash
tr 'a-z' 'A-Z' < filename
```

# 10. Replace spaces with underscores
```bash
tr ' ' '_' < filename
```

# 11. Print the first 10 lines of a file
```bash
head filename
```

# 12. Print the last 10 lines of a file
```bash
tail filename
```

# 13. Print only lines matching a specific pattern
```bash
awk '/pattern/ {print}' filename
```

# 14. Extract a specific field (e.g., 2nd field) from a file with columns
```bash
awk '{print $2}' filename
```

# 15. Display the number of occurrences of each word in a file
```bash
awk '{for(i=1;i<=NF;i++) w[$i]++} END{for(k in w) print k, w[k]}' filename
```

# 16. Sort by numeric value (ascending)
```bash
sort -n filename
```

# 17. Sort by numeric value (descending)
```bash
sort -nr filename
```

# 18. Remove empty lines from a file
```bash
grep -v '^$' filename
```

# 19. Find the number of occurrences of a word in a file
```bash
grep -o 'word' filename | wc -l
```

# 20. Display specific lines from a file (e.g., line 10 to 20)
```bash
sed -n '10,20p' filename
```