class Solution(object):
    def isValid(self, s):
        bracket_map = {")": "(", "}": "{", "]": "["}
        stack = []
        for char in s:
            if char in bracket_map:
                top_element = stack.pop() if stack else '#'            
                if bracket_map[char] != top_element:
                    return False
            else:
                stack.append(char)
        if len(stack) == 0:
            return True
        else:
            return False
<img width="1919" height="926" alt="Screenshot 2026-03-06 213821" src="https://github.com/user-attachments/assets/bdbd7c62-f88a-41c3-923d-420c8d6bf580" />
