# python
def print_sum_of_number_for_multiple_range(number , no_of_range):
    for i in range(no_of_range):
        from_range,to_range = map(int, input().split())
        sum_of_number = get_the_sum_of_number(number,from_range, to_range)
        print(sum_of_number)
        
def get_the_sum_of_number(number,from_range,to_range):
    sum_of_number=0 
    for each_number in number :
        if each_number >= from_range and each_number <= to_range :
            sum_of_number += each_number 
    return sum_of_number
    
def main():
   number = list(map(int,input().split()))
   no_of_range = int(input())
   print_sum_of_number_for_multiple_range(number,no_of_range)
   
main()
