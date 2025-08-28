# Lab01_315
First lab 1 of 315 based on dictionary bench marks
# Dictionary Benchmark

## Mannys ReadMe
Emmanuel Torbor - 008281371 - https://github.com/MannyTorbor/Lab01_315#
I have uploaded the zip file.
I had assisntance from chatgpt/google just asking for help on why it was taking 
each sort/unsort long and if its ok for it to take that long
Other than that it is my work and I used knowledge of my OWN past labs ive done for insert/remove functions 
Unsorted Vector I believe works: with this stest case: Unsorted Vector [N=5000] — Insert: 442us, Avg Lookup: 22503ns
Sorted vector works and I dont know if tis optimal time but it does output Sorted Vector [N=5000] — Insert: 2120us, Avg Lookup: 20468ns
Works and the output I got can vary though. Unsorted Linked List [N=5000] — Insert: 195us, Avg Lookup: 13610ns
Sorted Linked List [N=5000] — Insert: 22710us, Avg Lookup: 10144ns
Unsorted Vector [N=500000] — Insert: 34401us, Avg Lookup: 1975504ns
Sorted Vector [N=500000] — Insert: 6895946us, Avg Lookup: 2057762ns
Unsorted Linked List [N=500000] — Insert: 26158us, Avg Lookup: 1960600ns
For some reason my Sorted Linked List is the longest and takes a lot of time and I truly mean a long time for more than 10 minutes.
Which makes me think it techinically does not work as we should atleast be trying to get the most effective time.
## Structure

- `src/`: Contains `Dictionary` interface and `UnsortedVectorDict` implementation.
- `.github/workflows/test.yml`: GitHub Actions CI setup.

## How It Works

1. UnsortedVectorDict.cpp is complete and the main function contains the necessary code to test it. 
2. The output provides the average run-time for the **insert** and **lookup** function. However, only the average run-time values for the unsorted vector variation is meaningful as the other variations have not been implemented yet. But It is now implemented and run all test cases.
3. GitHub Actions runs 

## Run Locally

```bash
mkdir build && cd build
cmake ..
make
ctest --output-on-failure
```
