Is for make a rag
types of rags
- graph knowlage base
It search relationships in graph database
- Reranking rag
- Agentic rag  
The agent know how to search the information
- contextual retrival
 enrich each chunk with a llm, and it says how the chunk connect with the rest of the data
- query expancion
Improve the query for a rag
- Multy Query rag
Make multiples questions from a original questions
- context Aware chunking
Split the document for find the natual boudings of our documents 
- hierarchical rag
Is a kind of agentig rag with beheivor as a balanced tree
- self reflective aproch
it call 2 llms and the answers are evaluted by other llm 
- Fine tunned embedings
do a fine tunnig for specific user case

What is the process ?
Chunk the document, why we save the embedings in redis
we add to the enbedings more information


what is **Agentic Rag**

the agent take an active rol, it know in witch database search

Topics
python
Aws foundamentals (Amazon bedrock)
AI/Llm

past interview
map reduce
agentic rag
Agent2Agent protocol


Map reduce examples

1)

t=int(input())

map_out=[]
map_dict=dict()
for _ in range(t):
    text=input().split()
    for i in text:
        map_out.append((i,1))
#print(map_out)
for i in map_out:
    #print(i,i[0],i[1])

    if i[0] in map_dict:
        map_dict[i[0]] += i[1] 
    else:
        map_dict[i[0]] = i[1]
    #print(map_dict)    
    
print(map_dict)


2)
t = int(input())

map_out = []
map_dict = dict()
for _ in range(t):
    text = input().split(",")
    try:
        temp = float(text[1])
        map_out.append((text[0], temp))
    except:
        pass
print(map_out)
for i in map_out:
    # print(i,i[0],i[1])
    if i[0] in map_dict:
        map_dict[i[0]][1] += 1
        map_dict[i[0]][0].append(i[1])
    else:
        map_dict[i[0]] = [[i[1]], 1]
print(map_dict)
for i in map_dict:
    print(i, sum(map_dict[i][0]) / map_dict[i][1])



LLM 
values Temperature
from 0 to 2, is randomnes
Top-K `1` to 100, high values more creativity and low less creativity
Presence Penalty, if a token is repeted punish it
Stop Sequences
Frequency Penalty, punish if  a token is very often repeted 
Max Tokens