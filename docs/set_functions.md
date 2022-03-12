Various built-in functions are available in Python which helps to perform multiple operations on sets. Below are the top must know set methods in python

## **Length**
This function helps to return the length of the given set 

    #Length Method
    month_list = {"Jan", "Feb", "Mar", "Apr", "May"}
    print("Length of given set is: {}".format(len(month_list)))

 Output

    Length of given set is: 5

## **Set Union**
This helps to returns the union results of two sets

    #Set Union
    month_list_old = {"Jan", "Feb", "Mar"}
    month_list_new = {"Jan", "Feb", "Apr"}
    print("The union result of given two sets are")
    print(month_list_old | month_list_new)

 Output

    The union result of given two sets are
    {'Apr', 'Feb', 'Mar', 'Jan'}

## **Set Intersection**
This helps to return the intersection results of given sets

    #Set Intersection
    month_list_old = {"Jan", "Feb", "Mar"}
    month_list_new = {"Jan", "Feb", "Apr"}
    print("The intersection result of given two sets are")
    print(month_list_old & month_list_new)

 Output

    The intersection result of given two sets are
    {'Jan', 'Feb'}

## **Set Difference**
This helps to return the set difference of one set from another set

    #Set Difference
    month_list_old = {"Jan", "Feb", "Mar"}
    month_list_new = {"Jan", "Feb", "Apr"}
    print("The set difference of one set from another set is")
    print(month_list_old - month_list_new)

 Output

    The set difference of one set from another set is
    {'Mar'}

