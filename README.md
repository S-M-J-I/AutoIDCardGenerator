# Auto ID Card Generator

This is an auto ID card generator program. This will read an excel file and find the picture from the google drive from each row and create an ID card with the template ad shown below: 


The picture of the ID card: \
<img src='idCard.png' width='500px'></img>

### Steps:
- Load the member datasheet file
  - NOTE: while loading the file, ensure there are 4 fixed columns: **Name**, **ID**, **Email Address**, **Blood Group**, **Member Type** (with these headers)
- Download the images as a directory and place it in the root directory with this file. The path for one image **MUST** be accessible as `imgs/109230249.png`
- In the `generate()` function, pass the filename you want to generate the ID cards from.
  - `generate(filename(string), test=False(boolean), length=10(integer))`
    - `filename`: the path of the excel file
    - `test`: optional, if you want to conduct a test on the data to see its output
    - `length`: optional and works with `test`, set the range of test examples you want to generate