
### Background
Coding task

You have been given hourly solar weather data originating from a number of stations in CSV format. The data encompasses many years. This data exists across two files:

Weather data - tmy3.csv
Station metadata - TMY3_StationsMeta.csv


The exercise

Read the input data
Calculate the average GHI (W/m^2) and DNI (W/m^2) for each weather station at a weekly interval
Write the output to a .json file
The output file should have the following format where ghi and dhi are the average values for the respective measurement columns over the course of that week. Timestamp should the be time of the measurement week in MS since epoch.


```json
[
{
"id": "the weather station ID or USAF",
"site_name": "the weather station site name",
"coordinates": [150, -26],
"data": [
{
"timestamp": 1724703772146,
"ghi": 0,
"dni": 0
}
]
}
]
```


Tips

Choose the programming language and technology your are most familiar with.
Keep it simple: you should not need any additional infrastructure beyond your computer and your chosen language.
Document how to reproduce the results for the exercise (e.g how to run your program or binary)


Submission

Submit your code, along with a sample of the output file to a public git repository and share it.

Email us with a link to your repo at least one business day before the review meeting.

### Dependencies

- Python 3.11
- Software capable of running Jupyter Notebooks


### Environment setup

0. Navigate to project directory in shell

1. Create a new venv (called .venv):

```shell
python -m venv .venv				# create the environment
```

2. Activate that same virtual environment each time you create a shell window or session:

```shell
source .venv/bin/activate			# activate the environment for Mac and Linux .venv\Scripts\activate			# activate the environment for Windows
```

3. Install dependencies

```shell
pip install -r requirements.txt
```

4.To get .venv to work in jupyter notebook :

```shell
ipython kernel install --user --name=.venv
```
Select .venv kernel before running Jupyter notebook


### Reproducing results

1. run all cells in code-design-interview.ipynb

