# Stacks & Queues
# Stacks
![check](https://i.ibb.co/n1t6Xfr/stack.png)

## Stacks Concepts:
    1. **FILO:** Last In First Out :This means that the first item added in the stack will be the last item popped out of the stack.

    2. **LIFO:** Last In First Out :This means that the last item added to the stack will be the first item popped out of the stack.

* **stack is a data structure** that consists of **Nodes**.
* Each Node references the next Node in the stack, but does not reference its previous.
* Common terminology for a stack is
* **Push** : Nodes or items that are put into the stack are pushed
* **Pop** : Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
* **Top** : This is the top of the stack.
* **Peek** : When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
* **IsEmpty** : returns true when stack is empty otherwise returns false.
* When you push something to the stack, it becomes the new top
* When you pop something from the stack, you pop the current top and set the next top as ``top.next``.

## Push O(1)
* **Pushing a Node** onto a stack will always be an **O(1)** operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.
* When adding a Node, you push it into the stack by assigning it as the new top, with its next property equal to the original top.


## Pop O(1)
* Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.
* Typically, you would check isEmpty before conducting a pop. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block


## Peek O(1)
* When conducting a peek, you will only be inspecting the top Node of the stack.
* you would check isEmpty


# Queue
![check](https://i.ibb.co/K9sXwrY/que.png)

## Stacks Concepts:
    1. **FILO:** Last In First Out :This means that the first item in the queue will be the first item out of the queue.

    2. **LIFO:** Last In First Out :This means that the last item in the queue will be the last item out of the queue.


* **Enqueue** - Nodes or items that are added to the queue.
* **Dequeue** - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
* **Front** This is the front/first Node of the queue.
* **Rear**This is the rear/last Node of the queue.
* **Peek**When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
* **IsEmpty** - returns true when queue is empty otherwise returns false.
