Narrative Report: PHP Class Implementation (Activities 1 & 2)

This report presents an analysis of two PHP code examples (Activity 1 and Activity 2), both demonstrating the creation and utilization of classes to represent data. The report will assess the code's structure, functionality, and potential improvements.

Activity 1: The Product Class

![image](https://github.com/user-attachments/assets/cc2fedaa-3885-4504-ada4-fc59a25b3a12)

![image](https://github.com/user-attachments/assets/5a1cb5d4-e51a-4166-a40f-4c750e88b799)

Activity 1 introduces a Product class designed to encapsulate product information. The class defines five public properties: name , price , category , description , and stock . While the use of public properties simplifies access, it compromises data integrity. In a production environment, private properties with corresponding getter and setter methods would be preferable to ensure controlled access and data validation.

The class includes two methods:

setProduct() : This method acts as a constructor, assigning values to the product's properties. The order of arguments is critical and must align with the property order in the class definition. A more robust approach would involve using named parameters or an associative array to enhance readability and reduce the risk of errors.
getProductInfo() : This method returns a formatted string containing the product's details. The use of newline characters ( \n ) improves readability. The output is directly printed using echo . More sophisticated formatting techniques could be employed to enhance presentation.
The example instantiates a Product object for a "Smartphone" and prints its details. The output is clear and functional.

Activity 2: The Movie Class

![image](https://github.com/user-attachments/assets/befea0bb-fbb2-4207-9659-bdde6d53fc6a)

![image](https://github.com/user-attachments/assets/4857e3e8-1db5-49ea-b0a3-a6fb66507b87)

Activity 2 presents a Movie class, mirroring the structure of Activity 1 but focusing on movie-related data. The class includes public properties for title , genre , director , releaseYear , and duration . The same concerns regarding data integrity and the use of public properties apply here as in Activity 1.

The Movie class also includes two methods:

setMovie() : This method initializes the movie object's properties. Similar to setProduct() , the argument order is crucial and could be improved using named parameters or an associative array.
getMovieInfo() : This method returns a formatted string containing the movie's details. The formatting is more concise than in Activity 1, presenting all information on a single line. The output is printed using print() .
The example creates a Movie object for "Titanic" and prints its details.

Overall Assessment and Recommendations

Both activities successfully demonstrate the basic principles of class creation and object instantiation in PHP. However, the reliance on public properties necessitates improvements for better data security and maintainability. The use of private properties with getter and setter methods is strongly recommended. Furthermore, using named parameters or associative arrays for the setProduct() and setMovie() methods would enhance code readability and reduce the risk of errors. Finally, exploring more sophisticated formatting techniques in the getProductInfo() and getMovieInfo() methods would improve the presentation of the output. These improvements would significantly enhance the robustness and maintainability of the code.

Submitted By:
   Arlyne Joy Udaundo
