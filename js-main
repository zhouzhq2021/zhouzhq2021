/* 
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/ClientSide/javascript.js to edit this template
 */
var back = [
    [0, 1, 0, 1, 0, 1, 0, 1],
    [1, 0, 1, 0, 1, 0, 1, 0],
    [0, 1, 0, 1, 0, 1, 0, 1],
    [1, 0, 1, 0, 1, 0, 1, 0],
    [0, 1, 0, 1, 0, 1, 0, 1],
    [1, 0, 1, 0, 1, 0, 1, 0],
    [0, 1, 0, 1, 0, 1, 0, 1],
    [1, 0, 1, 0, 1, 0, 1, 0]];
//Define two-dimensional array to achieve checkerboard location

function getCellID(colsPerRow, r, c) {
    var id = r * colsPerRow + c;
    return "c" + id;
}//Creates the checkerboard function

function drawGameBoard(rows, cols) {
     var member1 = document.getElementById("member1");//Define the member variable
    member1.innerText = "Shengjie Xia";//Dispaly the member variable 
    var boardElement = document.getElementById("board");//Display the checkerboard
    var tableElement = document.createElement('table');//Create tableElement with table（attach to table）
    for (var i = 0; i < rows; i++) {
//This rows-loop is executed eight times
        var trElement = document.createElement('tr');//Create tableElement with tr（attach to tr）
        for (var j = 0; j < cols; j++) {
    //This tr-loop is executed eight times
            var tdElement = document.createElement('td');//Create tableElement with td（attach to td）
            var cellID = getCellID(8, i, j);//Utilize getCellID function
            tdElement.setAttribute('id', cellID);//Use setAttribute in the DOM tree to define the id attribute value 
            trElement.appendChild(tdElement);//Td's style is passed to tr using appendChild of the DOM tree  
            if (back[i][j] === 1)
                tdElement.className = 'white';//TdElement changes the class style to white  
            else
                tdElement.className = 'black';//TdElement changes the class style to black
        }
        tableElement.appendChild(trElement);//Pass the tr style to table  
    }
    boardElement.appendChild(tableElement);//Pass the table style to board   
}
