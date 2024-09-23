class Solution:  
    def solution(self, list1):  
        list1.sort()  
        for i in range(1, len(list1)):  
            for j in range(0, i):  
                if list1[i] == list1[i-1]:  
                    return 'true'  
            return 'false'  
  
obj = Solution()                 
list1 = [1, 2, 3, 1]  
print(obj.solution(list1))      
