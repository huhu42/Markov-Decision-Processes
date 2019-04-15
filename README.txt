CS 7641 Machine Learning - Markov Decision Processes

All codes are stored on GitHub at the following location: 


This code is adapted from code by mmallo3, from the following location:
https://github.gatech.edu/mmallo3/CS7641_Project4

To Run:

1. This project uses Python 3.6. Install all required packages in requirements.txt
2. To adjust/tune parameters, go to run_experiments.py. 
3. To run the project, from the project directory:
	python run_experiment.py --all
4. To plot:
	python run_experiment.py --plot
5. Output folder will be created and output files will be appended in the respective folders

Other available arguments for run_experiment.py:
	--threads 	Number of threads (default -1)
	--seed 		Set random seed
	-- policy	Run the Policy Iteration experiment only
	-- value	Run the Value Iteration experiment only
	-- ql		Run the Q-learning experiment only
	--verbose	Default to False, if true, verbose output
	-- help		help messages

Experiments include:
1. 4*12 Cliff Walking Experiment
2. 8*8 Frozen Lake Experiment
3. 15*15 Frozen Lake Experiment

To run the deterministic version of the experiment, go to run_experiment.py, change 'step_prob' to 1.0 and 'wind_prob' to 0 within the ENV_REWARDS set up. 
Re-name of old output folder, re-run the experiment with 'python run_experiment.py --all --plot'. 


