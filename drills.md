1a) Determine the Big O for the following algorithm: 
You are sitting in a room with 15 people. 
You want to find a playmate for your dog, preferably of the same breed. 
So you want to know if anyone out of the 15 people have the same breed as your dog. 
You stand up and yell out, who here has a golden retriever and would like to be a playdate for my golden. 
Someone yells - "I do, be happy to bring him over"

ANSWER: O(1) Input is 15, but he only had to ask 1x

1b) Determine the Big O for the following algorithm: 
You are sitting in a room with 15 people. 
You want to find a playmate for your dog who is of the same breed. 
So you want to know if anyone out of the 15 people have the same breed as your dog. 
You start with the first person and ask him if he has a golden retriever. 
He says no, then you ask the next person, and the next, and the 
next until you find someone who has a golden or there is no one else to ask.

ANSWER: O(15) Worst case is linear time, each time the increases you have another person to ask



2) Even or Odd
What is the Big O of the following algorithm? Explain your answer
function isEven(value) {
    if (value % 2 == 0) {
        return true;
    }
    else
        return false;
    }
} 
ANSWER: O(1) arithmetic operations are constant time



3) Are you Here?
What is the Big O of the following algorithm? Explain your answer

function areYouHere(arr1, arr2) {
    let ticket = 0, result = false;
    for (let i = 0; i < arr1.length; i++) {
        ticket++;
        const el1 = arr1[i];
        for (let j = 0; j < arr2.length; j++) {
            ticket++;
            const el2 = arr2[j];
            if (el1 === el2) 
                result: true;
        }
    }
    return {result: result, ticket: ticket};
}

ANSWER: O(arr1.length^arr2.length)


4) Doubler:
What is the Big O of the following algorithm? Explain your answer

function doubleArrayValues(array) {
    for (let i = 0; i < array.length; i++) {
        array[i] *= 2;
    }
    return array;
}

ANSWER: O(array.length) linear time - every item added to the array adds another operation

5) Naive serach
function naiveSearch(array, item) {
    for (let i = 0; i < array.length; i++) {
        if (array[i] === item) {
            return i;
        }
    }
}

ANSWER: O(array.length) - linear time - every item added to the array adds another operation


6) Creating Pairs
function createPairs(arr) {
    for (let i = 0; i < arr.length; i++) {
        for(let j = i + 1; j < arr.length; j++) {
            console.log(arr[i] + ", " +  arr[j] );
        }
    }
}

ANSWER: O(arr.length^2) polynomial


