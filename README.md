    Requirements
Libraries:
pandas
matplotlib
seaborn
plotly.express (optional for additional interactive visualizations)
How to Run
Ensure you have the required libraries installed.
Load the dataset from the specified path.
Execute the provided code snippets to generate the visualizations.
Notes
Adjust the file path for the CSV file as needed.
Modify plot parameters to suit specific requirements or preferences.
This README provides a concise description of the visualizations created and the steps to reproduce them.
sample code 

state_counts = df['State'].value_counts().head(10)
plt.figure(figsize=(12, 6))
sns.barplot(x=state_counts.index, y=state_counts.values, palette="viridis")
plt.title('Count of Electric Vehicles by State')
plt.xlabel('State')
plt.ylabel('Count')
plt.xticks(rotation=45)
plt.show()
