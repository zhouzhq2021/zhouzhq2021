/* 
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/ClientSide/javascript.js to edit this template
 */
function random(min, max) {
    return Math.floor(Math.random() * max) === 0 ? 1 : Math.floor(Math.random() * max);
}//Defining a random function
var order = 0;//Define variable order

function randomMove() {
    var r1 = 0;//Define variable r1
    var c1 = 0;//Define variable c1
    var m = 0;//Define variable m
    var n = 0;//Define variable n
     var member3 = document.getElementById("member3");
    member3.innerText = "Song Zichen";//Display the member
    if ((order % 2) === 0) {
        while (1) {
            r1 = random(0, 8);//r1 can be a number between 0 to 7
            c1 = random(0, 8);//c1 can be a number between 0 to 7
            if (pieces[r1][c1] == 1) {//if piece is black,then carry out this
                var x = r1 - 1;//Assign r1-1 to x
                if (x < 0) continue;
                var y0 = c1 + 1;//Assign c1+1 to y0
                var y1 = c1 - 1;//Assign c1-1 to y1
                if (random(0, 2) === 0) {//The syntax below is to ensure that the pieces move correctly and do not go out of bounds
                    if ((y0 >= 0 && y0 < 8) && pieces[x][y0] != 1) {
                        m = x;
                        n = y0;
                        break;
                    } else {
                        if ((y1 >= 0 && y1 < 8) && pieces[x][y1] != 1) {
                            m = x;
                            n = y1;
                            break;
                        }
                    }
                } else {
                    if ((y1 >= 0 && y1 < 8) && pieces[x][y1] != 1) {
                        m = x;
                        n = y1;
                        break;
                    } else {
                        if ((y0 >= 0 && y0 < 8) && pieces[x][y0] != 1) {
                            m = x;
                            n = y0;
                            break;
                        }
                    }
                }
            }
        }
        var cell1 = document.getElementById(getCellID(8, r1, c1));
        var cell2 = document.getElementById(getCellID(8, m, n));
        cell1.className = 'white';
        cell2.className = 'blackpiece';
        pieces[m][n] = 1;
        pieces[r1][c1] = 0;
    } else {
        while (1) {
            r1 = random(0, 8);//r1 can be a number between 0 to 7
            c1 = random(0, 8);//c1 can be a number between 0 to 7
            if (pieces[r1][c1] === -1) {//The syntax below is to ensure that the pieces move correctly and do not go out of bounds
                var x = r1 + 1;
                if (x < 0) continue;
                var y0 = c1 + 1;
                var y1 = c1 - 1;
                if (random(0, 2) === 0) {
                    if ((y0 >= 0 && y0 < 8) && pieces[x][y0] !== -1) {
                        m = x;
                        n = y0;
                        break;
                    } else {
                        if ((y1 >= 0 && y1 < 8) && pieces[x][y1] !== -1) {
                            m = x;
                            n = y1;
                            break;
                        }
                    }
                } else {
                    if ((y1 >= 0 && y1 < 8) && pieces[x][y1] !== -1) {
                        m = x;
                        n = y1;
                        break;
                    } else {
                        if ((y0 >= 0 && y0 < 8) && pieces[x][y0] !== -1) {
                            m = x;
                            n = y0;
                            break;
                        }
                    }
                }
            }
        }
        var cell1 = document.getElementById(getCellID(8, r1, c1));
        var cell2 = document.getElementById(getCellID(8, m, n));
        cell1.className = 'white';
        cell2.className = 'redpiece';
        pieces[m][n] = -1;
        pieces[r1][c1] = 0;
    }
     order++;  //Make sure Red and Black are moving alternately
}

