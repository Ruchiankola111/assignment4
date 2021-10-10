# assignment4

func secondLargestElement(a:[Int]) -> Int
 {
  var largest = 0
  var second_largest = 0

   for index in 0..<a.count
   {
      let val = a[index]

      if val > largest {
          second_largest = largest
          largest = val
      }else if val > second_largest, val != largest 
      {
            second_largest = val
      }
    }
    return second_largest
}
print(secondLargestElement(a: [43, 5, 1, 14, 3, 8, 72, 4, 6]))
              
            
