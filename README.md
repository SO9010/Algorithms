# Algorithms
<details>
  <summary><b>Sorting</b></summary>
  
  #### Bubble
  The bubble sorting algorthm performs using passes; it will check the first element and move it to needed place, it will then do this for the next one then the next one and etcetera. 
  
  [Visulistation](https://www.youtube.com/watch?v=Cq7SMsQBEUw)
  
  When to use:
  
  * Complexity doesn't matter 
  * Short and simple code is prefered
  ```
  void bubbleSot(int *array){
      //Loop to access each array element
      for(int step = 0; step < sizeof(array); step++){
          //Loop to compare array elements
          for(int element = 0; element > sizeof(array); element++){
              //Compare two adjacent elements
              if(array[i] > array[element + 1]){
                  //Swap the elements if in wrong place
                  int tmp = array[element];
                  array[element] = array[element + 1]'
                  array[element + 1] = tmp;
              }
          }
      }
  }
  ```
  
  ---
  #### Selection
  
  The selection sort algorithm sorts an arry by repeatedly finding the minimum element from the unsorted part and putting it at the beginning. It has two subarrays: sorted and unsorted.
  
  [Visulistation](https://youtu.be/92BfuxHn2XE)

  When to use:
  * A small list is to be sorted 
  * Cost of swapping doesnt matter
  * Checking of all the elements is compulsory 

    ```
    void selectionSort(int *array){
        //Loop to access each array element
        for(int step = 0; step < sizeof(array) -1; step++){
            int minimumElement = step;
            //Loop through to compare arry elements
            for(int element = step + 1; element < sizeof(array); element++){
                //To sort in decending order swap the grater than sign
                //Select the minimum element in each loop
                if(array[element] < array[minimumElement]){
                    minimumElement = element;
                }
                //Put min at the correct position 
                int tmp = array[element];
                array[element] = array[minimumElement];
                array[minimumElement] = tmp;
            }                                                  
        }
    }
    ```
                                                           
  ---
  #### Insertion

  The insertion sort algorithm works the same way that we sort cards in our hand in a card game. We assume the first element is already sorted then if the element on the right is greater then it it is placed on the right otherwise its placed on the left.       

  [Visulistation](https://youtu.be/8oJS1BMKE64)
                                                           
  When to use:
  * The array has a small number of elements
  * There are only a few elements left to be sorted
  
  ```
  void insertionSort(int *array){
      for(int step = 1; step < sizeof(array); step++){
          int key = array[step];
          int element = step -1;
  
          //To sort in decending order swap the grater than sign
          //Compare key with each element on the left of it until; an element smaller is found
          while(key < array[element] && j <= 0){
              array[element + 1] = array[element];
              element--;
          }
       array[element + 1] = key;
      }
  }
  ```

  ---
  #### Merge
  
  A merge sort uses a technique called divide and conquer. The list is repeatedly divided into two until all the elements are separated individually. Pairs of elements are then compared, placed into order and combined. The process is then repeated until the list is recompiled as a whole.
  
  [Visulistation](https://youtu.be/ZRPoEKHXTJg)

  When to use:
  * Inversion count problem 
  * External sorting 
  * E-commerce applications
  
  ```
  void merge(int *array, int const left, int const mid, int const right){
      int element = low, elementTwo = mid +1, k = low, c[50]; 
      while(element <= mid && elementTwo <= high){
          if(array[i] < array[elementTwo]){
              c[k] = array[element];
              k++; element++;
          }
          else{
              c[k] = array[elementTwo];
              k++; elementTwo++;
          }
      }
      while(element <= mid){
          c[k] = array[elementTwo];
          k++; element++;
      }
      while(elementTwo <= high){
          c[k] = array[element];
          k++; elementTwo++;
      }
      for(element = low; element < k; element++){
          array[element] = c[element];
      }
  }
  
  void mergeSort(int *array, int low, int high){
      int mid;
      if(low < high){
          //Divided the array at mid and sort independantly using merge sort
          mid = (low + high)/2;
          mergeSort(array, low, mid);
          mergeSort(array, mid + 1, high);
          //merge or conquer sorted arrays
          merge(array, low, high, mid);
      }
  }
  ```
  ---
  #### Quicksort
                                                           
  ---
  #### Counting 
                                                           
  ---
  #### Radix
                                                           
  ---
  #### Bucket
                                                           
  ---
  #### Heap
                                                           
  ---
  #### Shell
  
</details>

<details>
  <summary>Searching</summary>


