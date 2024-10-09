# COMP122 Lecture Notes: October 9, 2024

## Announcements:
   1. No Announcements


## Today's Agenda:

  1. Lecture
     - Introduction to Numbering System
       - Numbering Systems
       - Data Representation
       - Expanded Notation
       - Scientific Notation

  1. Lab
     - Multiplication Unit
     - Manually Testing 
     - Review of for-loop and if-then-else transformation/transliteration

## Questions from Last Lecture/Lab, etc.:
   * M/W 

    
   * T/R 


---
# Today's Lecture Material

  - Introduction to Numbering system
    * see slides: introduction-to-numbering-systems.pdf



# Today's Lab Material


  - Multiplication Unit
     ```mips
     mult rs, rt       #  {hi, lo} = rs * rt
     div  rs, rt       #  lo = rs / rt; hi = rs % rt 

     madd rs, rt       #  a = a + (rs * rt)
                       #  a is stored as {hi, lo}

     mflo rd           #  rd = lo
     mtlo rs           #  lo = rs
     mfhi rd           #  rd = hi
     mthi rs           #  hi = rs
     ```

  - Manually testing your code
    ```bash
    java_subroutine [-R null] {method} [{arg0}..{arg3}] [ <{input}] [ >{output}]
    ```
    - '[]' : indicates an optional within the command line
    - `-R null`  : prevents the printing of the return value of {method}
    - `{method}` : the name of the method you want to execute
    - `{arg0}..{arg3}` : optional command line arguments
    - ` <{input}`  : the input redirection of the named file
    - ` <{output}`  : the output redirection of the named file

  - Setup for the practicum
    - Directories:
      * Professors:
        - `PRACTICUM=code_10_09M`
        - `PRACTICUM=code_10_09A`
        - `PRACTICUM=code_10_10`
      * Suggested Student's directory to work along
        - `PRACTICUM=code_10_10_mine`

    - Commands
      ```bash
      history -c
      DST=~/classes/comp122/assembly-programming/${PRACTICUM}/
      cd ~/classes/comp122/assembly-programming
      git init ${PRACTICUM}
      cd ${PRACTICUM}
      pushd ~/classes/comp122/deliverables/simple-interest-{tab}
      cp -r bin java java_tac mips makefile test_cases ${DST}
      popd
      # Now we have everything to start!
      history -w my_history
      ls
      ```

  - Review of for-loop and if-then-else transformation/transliteration
    * see ~/classes/comp122/assembly-programming/code_10_09
      - java -> java_tac (transformation)
      - java_tac -> mips (transliteration)


---
## Resources
  * reference/TAC_transformation.md
  * reference/TAC_transformation/for-loop2TAC.md 
  * reference/TAC_transformation/if-then-else2TAC.md
  * reference/TAC2mips.md

---
<!-- This section for student's to place their own notes. -->
<!-- This section will not be updated by the Professor.   -->

## Notes  

