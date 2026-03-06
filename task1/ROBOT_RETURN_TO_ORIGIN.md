class Solution(object):
    def judgeCircle(self, moves):
        rcount=moves.count("R")
        lcount=moves.count("L")
        ucount=moves.count("U")
        dcount=moves.count("D")
        if lcount==rcount and ucount==dcount:
            return True
        else:
            return False
<img width="1917" height="926" alt="Screenshot 2026-03-06 211734" src="https://github.com/user-attachments/assets/7aeb7ae2-4457-4a39-a329-8b5e4c9676e5" />
