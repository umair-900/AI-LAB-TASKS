def check_result(score, documents, attendance, verification): 
 if score >= 70 and documents == True and attendance >= 75 and verification >= 60: 
return "Pass" 
else: 
return "Fail" 
test_cases = [ (85, True, 80, 75, "Pass", "All conditions are met"), (85, True, 70, 75, 
"Fail", "Attendance is less than 75"), (85, True, 80, 55, "Fail", "Verification score is less 
than 60"), (70, True, 75, 60, "Pass", "All values are exactly at the limit")] 
number = 1 
for case in test_cases: 
score = case[0] 
documents = case[1] 
attendance = case[2] 
verification = case[3] 
expected = case[4] 
reason = case[5] 
actual = check_result(score, documents, attendance, verification) 
print(f"Test Case {number}") 
print(f"Input: {(score, documents, attendance, verification)}") 
print(f"Expected: {expected}") 
print(f"Actual: {actual}") 
print(f"Reason: {reason}") 
print("-----------------------") 
number += 1 
Test Case 1 
Input: (85, True, 80, 75) 
Expected: Pass 
Actual: Pass 
Reason: All conditions are met. ----------------------- 
Test Case 2 
Input: (85, True, 70, 75) 
Expected: Fail 
Actual: Fail 
Reason: Attendance is less than 75. ----------------------- 
Test Case 3 
Input: (85, True, 80, 55) 
Expected: Fail 
Actual: Fail 
Reason: Verification score is less than 60. ----------------------- 
Test Case 4 
Input: (70, True, 75, 60) 
Expected: Pass 
Actual: Pass 
Reason: All values are exactly at the limit. ----------------------- 
Results 
Test Case 
Input 
Expected 
Actual 
Reason 
1 
(85, True, 80, 75) 
Pass 
Pass 
All conditions are met. 
2 
(85, True, 70, 75) 
Fail 
Fail 
Attendance is less than 75. 
3 
(85, True, 80, 55) 
Fail 
Fail 
Verification score is less than 60. 
4 
(70, True, 75, 60) 
Pass 
Pass 
All values are exactly at the limit.
