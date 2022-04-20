# labs
def calculateScore(person):
    if person == "kevin": t = 1 
    else: t = 0
    score = 0
    for i in range(len(s)):
        vocals = ['A', 'E', 'I', 'O', 'U']
        if vocals.count(s[i]) == t:         
            for j in range(i,len(s)-1):
                score += s.count(s[i:j+1])
    return(score)

def minion_game(s):
    s = calculateScore("kevin")
    p = calculateScore("stuart")
    
    if s > p: winner = "Kevin"
    else: winner = "Stuart"
    
    print(winner +" "+ str(max(s,p))) 

if __name__ == '__main__':
    s = raw_input()
    minion_game(s)
