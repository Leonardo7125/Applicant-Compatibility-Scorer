# Applicant-Compatibility-Scorer
This Python script reads in an input JSON file containing data about job applicants and team attributes, calculates the compatibility score between each applicant and the team, and outputs the scores for each applicant in a JSON format.

The compatibility score is calculated using the compatibility function, which takes two dictionaries as input: team and applicant. Each applicant dictionary contains a set of attributes and their corresponding values. The compatibility function iterates over each attribute in the team dictionary and calculates the compatibility score by taking the minimum value between the attribute value of the team and the applicant, and dividing it by 10.0. The resulting score is then added to the total score.

After the compatibility score for each applicant has been calculated, the code creates a list of scored applicants, each containing the name of the applicant and their corresponding compatibility score.

Finally, the code writes to an output JSON file, whose file name is based on the input file name, which contains the list of scored applicants. The console also prints a message indicating the file name that the data was saved to.
