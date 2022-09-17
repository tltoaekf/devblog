---
layout: post
title: "Organizing the code"
date: 2022-09-16 5:48:49 +0900
categories: Coding
---
​
## Introduction
​
---
​
Coding Organization: Change the color of cell, How to show the wrong cell & OOP
​
## Change the color of cell
​
```swift
  private func blinkAndAddNewCell() {
    //How to blink
    // 1. Red Cell -> Gray Cell
    // 2. Select new random cell
    // 3. Gray Cell -> Red Cell
    // takes 1Sec
    showColoredCells = false //Red Cell -> Gray Cell
    selectNextCellIndex() //Select new random cell
    
    DispatchQueue.main.asyncAfter(deadline: .now() + 1) { //takes 1Sec
      self.showColoredCells = true //Gray Cell -> Red Cell
    }
  }
```

## How to show the wrong cell

```swift
func checkUserSelection(userSelection: Int) {
    //If Correct -> Next Stage
    //If not correct -> bust: show green circle
    
    if userSelection == redCellIndices.last { //If Correct -> Next Stage
      //If there is another round -> go to the next round
      // if this is the last round, you win!
      //If there is another round -> go to the next round {
      if round == numberOfRows * numberOfRows - 1 {
        finishGame()
      } else {
        proceedToNextRound()
      }
    } else { // if wrong
      bustGame()
    }
  }
```


## OOP

```swift
OOP: Object-Oriented Programming
It seeks to understand a computer program as several independent units. Each object can send and receive messages and process data.
It has the advantages of making programming easier to learn, simplifying software development and maintenance, and enabling more intuitive code analysis.
//컴퓨터 프로그램을 여러 개의 독립된 단위로 파악하고자 하는 것이다. 각각의 객체는 메시지를 주고받고, 데이터를 처리할 수 있다. 프로그래밍을 더 배우기 쉽게 하고 소프트웨어 개발과 보수를 간편하게 하며, 보다 직관적인 코드 분석이 가능하다.
```

---
​
## Conclusion
​
Use true or false to decide if the program should go to the next step or not.
Use function to make the clear code. If you make a function once, you don't need to type code again. Call the function if you needed.
OOP seeks the program as an individual units. Each objects can process data.
