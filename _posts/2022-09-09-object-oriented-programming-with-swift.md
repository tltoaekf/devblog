---
layout: post
title: "Object oriented programming with Swift"
date: 2022-09-10 6:00:49 +0900
categories: Ideas
---
​
## Introduction
​
---
​
Introduce what you are going to explain in this article.
​
## View (or any other topic you want to write about)
​
```swift
let a = 3 // 1. 숫자 3을 a에 저장한다.
let b = 4 // 2. 숫자 4를 b에 저장한다.

let sum = a + b // 3. a와 b를 더하면 저장된 숫자들이 더해 진다. 여기서 값은 7이 나온다.
```
​
write summary and overall goal of the codes written above
​
## Image
​
```swift
  import SwiftUI
​
  struct ContentView: View {
      var body: some View {
          VStack { // 1. explain this line
              Image(systemName: "globe")
                  .imageScale(.large)
                  .foregroundColor(.accentColor) // 2. explain this line
              Text("Hello, world!") // 3. explain this line
              Image(uiImage: #imageLiteral(resourceName: "test"))
                  .resizable()
                  .scaledToFill()
                  .frame(width: 300, height: 300)
                  .background(Color.blue)
                  .clipShape(Circle()) // 4. explain this line
          }
      }
  }
​
```
​
write summary and overall goal of the codes written above
​
## Shape
​
```swift
​
  Enter swift code here
​
```
​
write summary and overall goal of the codes written above
​
---
​
## Conclusion
​
wrap up what you have learned today. 4-5 sentences.