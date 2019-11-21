
# Frequently useful commands

  - !<x> => repeat last command x with the parameters
  - !! => execute the last command
  - cd - => cd previous location and run pwd
  - pushd <dir> => push path to the stack 
  - popd <dir> => pop the path from the stack 
  - cd ~n => change directory to one in stack at n
  - dirs -v => show dirs stack
  - dirs -c => clear the stack 
    
 # Loops
 
  - until test-commands; do consequent-commands; done
  - while test-commands; do consequent-commands; done
  - for name [ [in [words ...] ] ; ] do commands; done
  - for (( expr1 ; expr2 ; expr3 )) ; do commands ; done

 # Conditional Constructs

   - if test-commands; then
    	consequent-commands;
    	[elif more-test-commands; then
    	more-consequents;]
    	[else alternate-consequents;]
     fi
   
   - case word in
    [ [(] pattern [| pattern]...) command-list ;;]...
    esac
   1)  *) is used as default case 
   2) ;; ends the case matching
   3) ;& continues with possible other cases
   
   - select name [in words ...]; do commands; done
   - 

 
# Array

  - declare -a ar 		# create an array 
  - ar[3]=escobar    		# create an array ands sets a value
  		                # indexed arrays start with 0
  - ${#arr[*]} 			# return the length of the array
  - ${ar[-1]} 			# value of the last ar, -2 would be second last item
  - echo "$ar[*]" 		# print the array with the $IFS
 
 - {1..10}	# numbers between 1 and 10 inclusive
 - {1..10..2} 	# numbers between 1-10 with step 2

# Arithmetics

- `expr 1 + 1` 		# evaluate the sum 
- `expr 2 \* 4`		# evaluate the product 
    
