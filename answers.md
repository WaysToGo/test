<table>
  <thead>
    <tr>
      <th>splice()</th>
      <th>slice()</th>      
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>returns the removed items</td>
      <td>returns the selected elements as a new array Object</td>      
    </tr>
    <tr>
      <td>Changes the original array </td>
      <td>does not change original array </td>     
    </tr>
    <tr>
      <td>takes **n** number of arguments</td>
      <td>takes **2** arguments</td>     
    </tr>
     <tr>
      <td>takes **n** number of arguments (start,deleteCount,items),deleteCount,items are optional</td>
      <td>takes **2** arguments (begin,end) Both are optional</td>     
    </tr>
     <tr>
      <td> ```javascript        
        var array=[1,2,3,4,5];
console.log(array.splice(2));
// [3, 4, 5], ->returns removed item(s) as a new array object.
        console.log(array);
// shows [1, 2], original array altered. 
var array2=[6,7,8,9,0];
console.log(array2.splice(2,1));
// shows [8] 
console.log(array2.splice(2,0));
//shows [] , as no item(s) removed.
 console.log(array2);
// shows [6,7,9,0] 
var array3=[11,12,13,14,15];
console.log(array3.splice(2,1,"Hello","World"));
// shows [13] 
console.log(array3);
// shows [11, 12, "Hello", "World", 14, 15] ```</td>       
      <td>
      ```javascript
      var array=[1,2,3,4,5]
console.log(array.slice(2));
// shows [3, 4, 5], returned selected element(s). 
console.log(array.slice(-2));
// shows [4, 5], returned selected element(s).
console.log(array);
// shows [1, 2, 3, 4, 5], original array remains intact. 
var array2=[6,7,8,9,0];
console.log(array2.slice(2,4));
// shows [8, 9] 
console.log(array2.slice(-2,4));
// shows [9] 
console.log(array2.slice(-3,-1));
// shows [8, 9] 
console.log(array2);
// shows [6, 7, 8, 9, 0]```</td>     
    </tr>    
  </tbody>
</table>
