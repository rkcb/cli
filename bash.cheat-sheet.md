
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
   - *) is used as default case 

   

