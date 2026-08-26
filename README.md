# peterbilt_hackathon

Peterbilt Truck Configuration Analysis: Identifying Warranty Cost Drivers

24-hour hackathon project analyzing Peterbilt truck build configurations and warranty claims to identify which attributes and attribute pairs drive up warranty costs, and building a model to flag high-risk configurations before they ship.

Problem

Peterbilt offers a wide range of build specs (8 attributes, 315 possible option codes) across its Heavy Duty trucks. The goal: pinpoint which options and option pairings are most associated with warranty claims, and build a model to predict claim risk for new configurations.

Approach

•Reliability scoring: Compared each option's overall score against its average claim cost to flag likely cost drivers  surfacing known problem areas like the 567 and 579 models.
•Interaction analysis: Tested attribute pairs (e.g., Attribute 1 & 4, Attribute 2 & 5) and found specific combinations with notably higher predicted warranty costs than either attribute alone.
•XGBoost model: Trained a classifier to predict claim risk from configuration attributes 84.4% accuracy, with strong precision/recall on identifying no-claim cases.


Key Findings

•567 and 579 configurations show recurring recall/claim patterns.
•Certain attribute pairs compound warranty risk beyond individual attributes.
•The model gives Peterbilt a practical way to flag risky configurations proactively, before they scale into costly recalls.


Note: This was designed as a 4-person team hackathon challenge. I competed solo, built the full analysis and model within the 24-hour window, and was selected as one of the top 5 teams out of 20 to present findings to the judging committee.
