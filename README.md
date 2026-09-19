# Merge_two_Sorted_arrays
This program takes two sorted arrays and combine them and convert it into one sorted arrays 


    
    
    def merge(arr1,arr2):
        sorted_combine_array=[]
        l=0
        r=0
        L1=len(arr1)
        L2=len(arr2)
        
        while l<L1 and r<L2:
            if arr1[l]<arr2[r]:
                sorted_combine_array.append(arr1[l])
                l+=1
            else:
                sorted_combine_array.append(arr2[r])
                r+=1
                
        sorted_combine_array.extend(arr1[l:])
        sorted_combine_array.extend(arr2[r:])
        return sorted_combine_array         

    arr1=list(map(int,input("Enter array 1 elements in Sorted Order with spaces between them : ").split()))
    arr2=list(map(int,input("Enter array 2 elements in Sorted Order with spaces between them : ").split()))
    
    
    print(" !....................... Thanks for providing the elements for both arrays in the Sorted Order ........... ! ")
    print()
    print("#"*109)
    print()
    
    print(f"The Sorted Combine Array is {merge(arr1,arr2)}")



    
    

