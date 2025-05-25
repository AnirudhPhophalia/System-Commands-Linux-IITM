**Question:**
 A company has 5 departments, each named `Dept1` to `Dept5`. Within each department, there are 3 teams labeled `
       │ TeamA` to `TeamC`. Each team works on 10 projects.
   2   │
   3   │ There is a directory for every team in `~/se2001/BPT1_problem_1/`.
   4   │
   5   │ **Write Bash command(s) to create a file for each project, with the files named from `project1` to `project10`,
       │  in every team directory. Each file should be empty to ensure minimal space usage.**

**Answer:**
for dept in {1..5}; do for team in A B C; do mkdir -p "Dept${dept}/Team${team}" && touch "Dept${dept}/Team${team}/project"{1..10}; done; done
