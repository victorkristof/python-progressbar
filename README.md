# Python Simple Progress Bar

A simple, easy-to-use progress bar for your time consuming operations.

## Usage
````
bar = ProgressBar(100)
bar.start()
for i in range(0, 100):
    time.sleep(1)
    bar.update(i)
````
Output:

````
Progress: [##########          ] 50%
````

## Documentation
### Basics
You set the end value and update it at each iteration with the new value. Please note that it assumes values from 0 to `end_value`-1.
### Customization
#### Bar length
You can set the length of the bar (hashes) by setting `bar_length`. Default: 20.
#### Info Text
You can set the informative text before the bar by setting `text`. Default: `"Progress"`.