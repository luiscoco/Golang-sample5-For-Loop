# Golang: Loops

![image](https://github.com/luiscoco/Golang-sample5-For-Loop/assets/32194879/2517d7c5-bb56-49db-941e-de6b0cb7ae05)

## 1. Source code

```go
package main

import (
	"fmt"
)

func main() {
	// Basic for loop
	fmt.Println("Basic for loop:")
	for i := 0; i < 5; i++ {
		fmt.Println(i)
	}

	// For loop as a while loop
	fmt.Println("\nFor loop as a while loop:")
	j := 0
	for j < 5 {
		fmt.Println(j)
		j++
	}

	// Infinite loop with break condition
	fmt.Println("\nInfinite loop with break condition:")
	k := 0
	for {
		if k >= 5 {
			break
		}
		fmt.Println(k)
		k++
	}

	// Using continue in a for loop
	fmt.Println("\nUsing continue in a for loop:")
	for l := 0; l < 5; l++ {
		if l%2 == 0 {
			continue
		}
		fmt.Println(l)
	}

	// Iterating over a slice with range
	fmt.Println("\nIterating over a slice with range:")
	numbers := []int{10, 20, 30, 40, 50}
	for index, value := range numbers {
		fmt.Printf("Index: %d, Value: %d\n", index, value)
	}

	// Iterating over a map with range
	fmt.Println("\nIterating over a map with range:")
	fruits := map[string]string{"a": "apple", "b": "banana", "c": "cherry"}
	for key, value := range fruits {
		fmt.Printf("Key: %s, Value: %s\n", key, value)
	}
}
```

## 2. How to run the application

```
go run loops.go
```

