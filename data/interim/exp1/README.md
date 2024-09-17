### wheel_data.csv
Some explanations of columns in wheel_data.csv: 
1. sona_id: the subject identifier
2. trial_index (can be ignored)
3. color-wheel: participant response on color wheel in degrees
4. shape-wheel: participant response on shape wheel in degrees
5. shape: the actual target shape in degrees
6. color: the actual target color in degrees
7. points: whether they got that item correct or incorrect
8. trial_for_match: can be ignored
9. correct rule numeric: maps rules to numbers from following dict 
    ```python
    rulemaps = {0: 'hot',1:'cold',2:'sharp',3:'round'} 
    ```
10. correct_rule: text version of the correct rule
11. prev_correct_rule: which rule was correct in the previous event
12. trial_within_block: what number trial the item was in an event
13. rel_subj_boundary: position to nearest boundary. Negative numbers are before boundary, positie after.
14. color_diff: how different the response was from the color 
15. shape_diff: how different the response was from the shape
16. color_diff_abs: absolute value of 14
17. shape_diff_abs: absolute value of 15
18. boundary_label: uses the following map 
    ```python
    boundary_map = {0:'boundary',1:'post_boundary',-1:'pre_boundary'}
    # if not in the boundary map it is set as non_boundary
    ```
