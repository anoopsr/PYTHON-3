def longestWords(WordsList):
    wordlength={}
    longwords=[]
    for word in WordsList:
        wordlength[word]=len(word)
    maxlength = max(wordlength.values())
    for key,value in wordlength.items():
        if(value == maxlength):
            longwords.append(key)
    return longwords 
WordsList = ['Bangalore','Kerala','Chennai','Tamilnadu','Delhi','Rajasthan','Punjab','Mumbai']
LongestWordsList = longestWords(WordsList)
print(LongestWordsList )
