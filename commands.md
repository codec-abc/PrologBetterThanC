```
sudo apt-get install swi-prolog
git submodule update --init --recursive
cd SudokuSolver
swipl -l solver.pl -t "solve_sudoku('../test_grid_prolog_program.txt','../sol_prolog.txt')."
cd ..
cd Parallel_Sudoku_Solver
make
./Parallel_Sudoku_Solver 1 ../test_grid_c_program.txt
cd ..
```