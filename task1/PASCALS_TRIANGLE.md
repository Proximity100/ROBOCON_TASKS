class Solution(object):
    def generate(self, numRows):
        triangle = [[1]]
        for i in range(1, numRows):
            prev_row = triangle[i-1]
            current_row = [1]
            for j in range(1, i):
                current_row.append(prev_row[j-1] + prev_row[j])
            current_row.append(1)
            triangle.append(current_row)
        
        return triangle
        <img width="1916" height="922" alt="Screenshot 2026-03-06 212548" src="https://github.com/user-attachments/assets/515164d8-cd92-4173-bdf7-b31395a8f26e" />
