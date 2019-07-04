
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
  - two loops: for x in $(ls); do for y in $(ls); do echo "$x $y"; done; done;
