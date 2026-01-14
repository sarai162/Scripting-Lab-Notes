# Assignment — Update todo.sh to sort entries and test

Update the `todo.sh` script to do the following:

1. Allow a user to add items interactively to a todo list.
2. When the user types `stop`, stop accepting input.
3. Print the current todo list.
4. Sort the todo items in alphabetical order and print the sorted list.
5. Test the script using these inputs (enter each on its own prompt):  
   Meditate  
   Hydrate  
   Work  
   Study  
   Exercise  
   Sleep

Remember: type `stop` when you are done adding items to the array.

## Script (todo.sh)

```bash
#!/bin/bash
declare -a todo_list
while read -p "Add items to your to do list (or type 'stop' to stop adding): " todo; do
  if [[ "${todo}" == "stop" ]]; then
    break
  fi
  todo_list+=("${todo}")
done
echo "Current todo list: ${todo_list[@]}"
sorted_array=$(printf "%s\n" "${todo_list[@]}" | sort)
printf "%s\n" "Sorted todo list:" ${sorted_array[@]}
```

## Example terminal session

```console
$ bash todo.sh
Add items to your to do list (or type 'stop' to stop adding): Meditate
Add items to your to do list (or type 'stop' to stop adding): Hydrate
Add items to your to do list (or type 'stop' to stop adding): Work
Add items to your to do list (or type 'stop' to stop adding): Study
Add items to your to do list (or type 'stop' to stop adding): Exercise
Add items to your to do list (or type 'stop' to stop adding): Sleep
Add items to your to do list (or type 'stop' to stop adding): stop
Current todo list: Meditate Hydrate Work Study Exercise Sleep
Sorted todo list:
Exercise
Hydrate
Meditate
Sleep
Study
Work
$
```
