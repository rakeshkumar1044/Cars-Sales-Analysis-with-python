Working on Real Project with Python (cars Dataset)
==================================================

(A Part of Big Data Analyst )

Cars Dataset

Cars Dataset Here, the data of Differenr is given with their
specifications.¶ this data is availables as CSV file, we are going to
analysze this data set using the pandas DataFrame.

.. code:: ipython3

    import pandas as pd 
    car=pd.read_csv(r"C:\Users\Dell\Desktop\Car Data Analyst\car.csv")

.. code:: ipython3

    car




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Make</th>
          <th>Model</th>
          <th>Type</th>
          <th>Origin</th>
          <th>DriveTrain</th>
          <th>MSRP</th>
          <th>Invoice</th>
          <th>EngineSize</th>
          <th>Cylinders</th>
          <th>Horsepower</th>
          <th>MPG_City</th>
          <th>MPG_Highway</th>
          <th>Weight</th>
          <th>Wheelbase</th>
          <th>Length</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>0</th>
          <td>Acura</td>
          <td>MDX</td>
          <td>SUV</td>
          <td>Asia</td>
          <td>All</td>
          <td>$36,945</td>
          <td>$33,337</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>265</td>
          <td>17</td>
          <td>23</td>
          <td>4451</td>
          <td>106</td>
          <td>189</td>
        </tr>
        <tr>
          <th>1</th>
          <td>Acura</td>
          <td>RSX Type S 2dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$23,820</td>
          <td>$21,761</td>
          <td>2.0</td>
          <td>4.0</td>
          <td>200</td>
          <td>24</td>
          <td>31</td>
          <td>2778</td>
          <td>101</td>
          <td>172</td>
        </tr>
        <tr>
          <th>2</th>
          <td>Acura</td>
          <td>TSX 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$26,990</td>
          <td>$24,647</td>
          <td>2.4</td>
          <td>4.0</td>
          <td>200</td>
          <td>22</td>
          <td>29</td>
          <td>3230</td>
          <td>105</td>
          <td>183</td>
        </tr>
        <tr>
          <th>3</th>
          <td>Acura</td>
          <td>TL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$33,195</td>
          <td>$30,299</td>
          <td>3.2</td>
          <td>6.0</td>
          <td>270</td>
          <td>20</td>
          <td>28</td>
          <td>3575</td>
          <td>108</td>
          <td>186</td>
        </tr>
        <tr>
          <th>4</th>
          <td>Acura</td>
          <td>3.5 RL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$43,755</td>
          <td>$39,014</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>225</td>
          <td>18</td>
          <td>24</td>
          <td>3880</td>
          <td>115</td>
          <td>197</td>
        </tr>
        <tr>
          <th>...</th>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
        </tr>
        <tr>
          <th>423</th>
          <td>Volvo</td>
          <td>C70 LPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$40,565</td>
          <td>$38,203</td>
          <td>2.4</td>
          <td>5.0</td>
          <td>197</td>
          <td>21</td>
          <td>28</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>424</th>
          <td>Volvo</td>
          <td>C70 HPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$42,565</td>
          <td>$40,083</td>
          <td>2.3</td>
          <td>5.0</td>
          <td>242</td>
          <td>20</td>
          <td>26</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>425</th>
          <td>Volvo</td>
          <td>S80 T6 4dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$45,210</td>
          <td>$42,573</td>
          <td>2.9</td>
          <td>6.0</td>
          <td>268</td>
          <td>19</td>
          <td>26</td>
          <td>3653</td>
          <td>110</td>
          <td>190</td>
        </tr>
        <tr>
          <th>426</th>
          <td>Volvo</td>
          <td>V40</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$26,135</td>
          <td>$24,641</td>
          <td>1.9</td>
          <td>4.0</td>
          <td>170</td>
          <td>22</td>
          <td>29</td>
          <td>2822</td>
          <td>101</td>
          <td>180</td>
        </tr>
        <tr>
          <th>427</th>
          <td>Volvo</td>
          <td>XC70</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>All</td>
          <td>$35,145</td>
          <td>$33,112</td>
          <td>2.5</td>
          <td>5.0</td>
          <td>208</td>
          <td>20</td>
          <td>27</td>
          <td>3823</td>
          <td>109</td>
          <td>186</td>
        </tr>
      </tbody>
    </table>
    <p>428 rows × 15 columns</p>
    </div>



.. code:: ipython3

    car.isnull().sum()




.. parsed-literal::

    Make           0
    Model          0
    Type           0
    Origin         0
    DriveTrain     0
    MSRP           0
    Invoice        0
    EngineSize     0
    Cylinders      2
    Horsepower     0
    MPG_City       0
    MPG_Highway    0
    Weight         0
    Wheelbase      0
    Length         0
    dtype: int64



1. Instruction (For data Cleaning)
==================================

Find all Null Values in the dataset. If there is any null values in any
columns ,then fill the mean of that columns.

.. code:: ipython3

    car.Cylinders.isnull().sum()




.. parsed-literal::

    2



.. code:: ipython3

    car.Cylinders.mean()




.. parsed-literal::

    5.807511737089202



.. code:: ipython3

    car.Cylinders.fillna(car.Cylinders.mean(),inplace=True)

.. code:: ipython3

    car.Cylinders.isnull().sum()




.. parsed-literal::

    0



.. code:: ipython3

    car.isnull().sum()




.. parsed-literal::

    Make           0
    Model          0
    Type           0
    Origin         0
    DriveTrain     0
    MSRP           0
    Invoice        0
    EngineSize     0
    Cylinders      0
    Horsepower     0
    MPG_City       0
    MPG_Highway    0
    Weight         0
    Wheelbase      0
    Length         0
    dtype: int64



2. Questions ( Based on value counts)
=====================================

Check what are different type of make are there in our dataset. And what
is the count (Occurrence ) of each Make I the data ?

.. code:: ipython3

    car.Make.unique()




.. parsed-literal::

    array(['Acura', 'Audi', 'BMW', 'Buick', 'Cadillac', 'Chevrolet',
           'Chrysler', 'Dodge', 'Ford', 'GMC', 'Honda', 'Hummer', 'Hyundai',
           'Infiniti', 'Isuzu', 'Jaguar', 'Jeep', 'Kia', 'Land Rover',
           'Lexus', 'Lincoln', 'MINI', 'Mazda', 'Mercedes-Benz', 'Mercury',
           'Mitsubishi', 'Nissan', 'Oldsmobile', 'Pontiac', 'Porsche', 'Saab',
           'Saturn', 'Scion', 'Subaru', 'Suzuki', 'Toyota', 'Volkswagen',
           'Volvo'], dtype=object)



.. code:: ipython3

    car.Make.nunique()




.. parsed-literal::

    38



.. code:: ipython3

    car.Make.value_counts()




.. parsed-literal::

    Make
    Toyota           28
    Chevrolet        27
    Mercedes-Benz    26
    Ford             23
    BMW              20
    Audi             19
    Honda            17
    Nissan           17
    Volkswagen       15
    Chrysler         15
    Dodge            13
    Mitsubishi       13
    Volvo            12
    Jaguar           12
    Hyundai          12
    Subaru           11
    Pontiac          11
    Mazda            11
    Lexus            11
    Kia              11
    Buick             9
    Mercury           9
    Lincoln           9
    Saturn            8
    Cadillac          8
    Suzuki            8
    Infiniti          8
    GMC               8
    Acura             7
    Porsche           7
    Saab              7
    Land Rover        3
    Oldsmobile        3
    Jeep              3
    Scion             2
    Isuzu             2
    MINI              2
    Hummer            1
    Name: count, dtype: int64



.. code:: ipython3

    #  with filter
    
    car[(car["Origin"]=="Asia") | (car["Origin"]=="Europe")]




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Make</th>
          <th>Model</th>
          <th>Type</th>
          <th>Origin</th>
          <th>DriveTrain</th>
          <th>MSRP</th>
          <th>Invoice</th>
          <th>EngineSize</th>
          <th>Cylinders</th>
          <th>Horsepower</th>
          <th>MPG_City</th>
          <th>MPG_Highway</th>
          <th>Weight</th>
          <th>Wheelbase</th>
          <th>Length</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>0</th>
          <td>Acura</td>
          <td>MDX</td>
          <td>SUV</td>
          <td>Asia</td>
          <td>All</td>
          <td>$36,945</td>
          <td>$33,337</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>265</td>
          <td>17</td>
          <td>23</td>
          <td>4451</td>
          <td>106</td>
          <td>189</td>
        </tr>
        <tr>
          <th>1</th>
          <td>Acura</td>
          <td>RSX Type S 2dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$23,820</td>
          <td>$21,761</td>
          <td>2.0</td>
          <td>4.0</td>
          <td>200</td>
          <td>24</td>
          <td>31</td>
          <td>2778</td>
          <td>101</td>
          <td>172</td>
        </tr>
        <tr>
          <th>2</th>
          <td>Acura</td>
          <td>TSX 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$26,990</td>
          <td>$24,647</td>
          <td>2.4</td>
          <td>4.0</td>
          <td>200</td>
          <td>22</td>
          <td>29</td>
          <td>3230</td>
          <td>105</td>
          <td>183</td>
        </tr>
        <tr>
          <th>3</th>
          <td>Acura</td>
          <td>TL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$33,195</td>
          <td>$30,299</td>
          <td>3.2</td>
          <td>6.0</td>
          <td>270</td>
          <td>20</td>
          <td>28</td>
          <td>3575</td>
          <td>108</td>
          <td>186</td>
        </tr>
        <tr>
          <th>4</th>
          <td>Acura</td>
          <td>3.5 RL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$43,755</td>
          <td>$39,014</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>225</td>
          <td>18</td>
          <td>24</td>
          <td>3880</td>
          <td>115</td>
          <td>197</td>
        </tr>
        <tr>
          <th>...</th>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
        </tr>
        <tr>
          <th>423</th>
          <td>Volvo</td>
          <td>C70 LPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$40,565</td>
          <td>$38,203</td>
          <td>2.4</td>
          <td>5.0</td>
          <td>197</td>
          <td>21</td>
          <td>28</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>424</th>
          <td>Volvo</td>
          <td>C70 HPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$42,565</td>
          <td>$40,083</td>
          <td>2.3</td>
          <td>5.0</td>
          <td>242</td>
          <td>20</td>
          <td>26</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>425</th>
          <td>Volvo</td>
          <td>S80 T6 4dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$45,210</td>
          <td>$42,573</td>
          <td>2.9</td>
          <td>6.0</td>
          <td>268</td>
          <td>19</td>
          <td>26</td>
          <td>3653</td>
          <td>110</td>
          <td>190</td>
        </tr>
        <tr>
          <th>426</th>
          <td>Volvo</td>
          <td>V40</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$26,135</td>
          <td>$24,641</td>
          <td>1.9</td>
          <td>4.0</td>
          <td>170</td>
          <td>22</td>
          <td>29</td>
          <td>2822</td>
          <td>101</td>
          <td>180</td>
        </tr>
        <tr>
          <th>427</th>
          <td>Volvo</td>
          <td>XC70</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>All</td>
          <td>$35,145</td>
          <td>$33,112</td>
          <td>2.5</td>
          <td>5.0</td>
          <td>208</td>
          <td>20</td>
          <td>27</td>
          <td>3823</td>
          <td>109</td>
          <td>186</td>
        </tr>
      </tbody>
    </table>
    <p>281 rows × 15 columns</p>
    </div>



.. code:: ipython3

    ###   with isin funtion
    car[car.Origin.isin(["Asia","Europe"])]




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Make</th>
          <th>Model</th>
          <th>Type</th>
          <th>Origin</th>
          <th>DriveTrain</th>
          <th>MSRP</th>
          <th>Invoice</th>
          <th>EngineSize</th>
          <th>Cylinders</th>
          <th>Horsepower</th>
          <th>MPG_City</th>
          <th>MPG_Highway</th>
          <th>Weight</th>
          <th>Wheelbase</th>
          <th>Length</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>0</th>
          <td>Acura</td>
          <td>MDX</td>
          <td>SUV</td>
          <td>Asia</td>
          <td>All</td>
          <td>$36,945</td>
          <td>$33,337</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>265</td>
          <td>17</td>
          <td>23</td>
          <td>4451</td>
          <td>106</td>
          <td>189</td>
        </tr>
        <tr>
          <th>1</th>
          <td>Acura</td>
          <td>RSX Type S 2dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$23,820</td>
          <td>$21,761</td>
          <td>2.0</td>
          <td>4.0</td>
          <td>200</td>
          <td>24</td>
          <td>31</td>
          <td>2778</td>
          <td>101</td>
          <td>172</td>
        </tr>
        <tr>
          <th>2</th>
          <td>Acura</td>
          <td>TSX 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$26,990</td>
          <td>$24,647</td>
          <td>2.4</td>
          <td>4.0</td>
          <td>200</td>
          <td>22</td>
          <td>29</td>
          <td>3230</td>
          <td>105</td>
          <td>183</td>
        </tr>
        <tr>
          <th>3</th>
          <td>Acura</td>
          <td>TL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$33,195</td>
          <td>$30,299</td>
          <td>3.2</td>
          <td>6.0</td>
          <td>270</td>
          <td>20</td>
          <td>28</td>
          <td>3575</td>
          <td>108</td>
          <td>186</td>
        </tr>
        <tr>
          <th>4</th>
          <td>Acura</td>
          <td>3.5 RL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$43,755</td>
          <td>$39,014</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>225</td>
          <td>18</td>
          <td>24</td>
          <td>3880</td>
          <td>115</td>
          <td>197</td>
        </tr>
        <tr>
          <th>...</th>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
        </tr>
        <tr>
          <th>423</th>
          <td>Volvo</td>
          <td>C70 LPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$40,565</td>
          <td>$38,203</td>
          <td>2.4</td>
          <td>5.0</td>
          <td>197</td>
          <td>21</td>
          <td>28</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>424</th>
          <td>Volvo</td>
          <td>C70 HPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$42,565</td>
          <td>$40,083</td>
          <td>2.3</td>
          <td>5.0</td>
          <td>242</td>
          <td>20</td>
          <td>26</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>425</th>
          <td>Volvo</td>
          <td>S80 T6 4dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$45,210</td>
          <td>$42,573</td>
          <td>2.9</td>
          <td>6.0</td>
          <td>268</td>
          <td>19</td>
          <td>26</td>
          <td>3653</td>
          <td>110</td>
          <td>190</td>
        </tr>
        <tr>
          <th>426</th>
          <td>Volvo</td>
          <td>V40</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$26,135</td>
          <td>$24,641</td>
          <td>1.9</td>
          <td>4.0</td>
          <td>170</td>
          <td>22</td>
          <td>29</td>
          <td>2822</td>
          <td>101</td>
          <td>180</td>
        </tr>
        <tr>
          <th>427</th>
          <td>Volvo</td>
          <td>XC70</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>All</td>
          <td>$35,145</td>
          <td>$33,112</td>
          <td>2.5</td>
          <td>5.0</td>
          <td>208</td>
          <td>20</td>
          <td>27</td>
          <td>3823</td>
          <td>109</td>
          <td>186</td>
        </tr>
      </tbody>
    </table>
    <p>281 rows × 15 columns</p>
    </div>



4. instruction (Removing unwanted record)
=========================================

Remove all the record (rows) where weight is above 4000.

.. code:: ipython3

    (car.Weight>4000).sum()




.. parsed-literal::

    103



.. code:: ipython3

    (car["Weight"]>4000).sum()




.. parsed-literal::

    103



.. code:: ipython3

    car.Weight>4000




.. parsed-literal::

    0       True
    1      False
    2      False
    3      False
    4      False
           ...  
    423    False
    424    False
    425    False
    426    False
    427    False
    Name: Weight, Length: 428, dtype: bool



.. code:: ipython3

    car




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Make</th>
          <th>Model</th>
          <th>Type</th>
          <th>Origin</th>
          <th>DriveTrain</th>
          <th>MSRP</th>
          <th>Invoice</th>
          <th>EngineSize</th>
          <th>Cylinders</th>
          <th>Horsepower</th>
          <th>MPG_City</th>
          <th>MPG_Highway</th>
          <th>Weight</th>
          <th>Wheelbase</th>
          <th>Length</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>0</th>
          <td>Acura</td>
          <td>MDX</td>
          <td>SUV</td>
          <td>Asia</td>
          <td>All</td>
          <td>$36,945</td>
          <td>$33,337</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>265</td>
          <td>17</td>
          <td>23</td>
          <td>4451</td>
          <td>106</td>
          <td>189</td>
        </tr>
        <tr>
          <th>1</th>
          <td>Acura</td>
          <td>RSX Type S 2dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$23,820</td>
          <td>$21,761</td>
          <td>2.0</td>
          <td>4.0</td>
          <td>200</td>
          <td>24</td>
          <td>31</td>
          <td>2778</td>
          <td>101</td>
          <td>172</td>
        </tr>
        <tr>
          <th>2</th>
          <td>Acura</td>
          <td>TSX 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$26,990</td>
          <td>$24,647</td>
          <td>2.4</td>
          <td>4.0</td>
          <td>200</td>
          <td>22</td>
          <td>29</td>
          <td>3230</td>
          <td>105</td>
          <td>183</td>
        </tr>
        <tr>
          <th>3</th>
          <td>Acura</td>
          <td>TL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$33,195</td>
          <td>$30,299</td>
          <td>3.2</td>
          <td>6.0</td>
          <td>270</td>
          <td>20</td>
          <td>28</td>
          <td>3575</td>
          <td>108</td>
          <td>186</td>
        </tr>
        <tr>
          <th>4</th>
          <td>Acura</td>
          <td>3.5 RL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$43,755</td>
          <td>$39,014</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>225</td>
          <td>18</td>
          <td>24</td>
          <td>3880</td>
          <td>115</td>
          <td>197</td>
        </tr>
        <tr>
          <th>...</th>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
        </tr>
        <tr>
          <th>423</th>
          <td>Volvo</td>
          <td>C70 LPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$40,565</td>
          <td>$38,203</td>
          <td>2.4</td>
          <td>5.0</td>
          <td>197</td>
          <td>21</td>
          <td>28</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>424</th>
          <td>Volvo</td>
          <td>C70 HPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$42,565</td>
          <td>$40,083</td>
          <td>2.3</td>
          <td>5.0</td>
          <td>242</td>
          <td>20</td>
          <td>26</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>425</th>
          <td>Volvo</td>
          <td>S80 T6 4dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$45,210</td>
          <td>$42,573</td>
          <td>2.9</td>
          <td>6.0</td>
          <td>268</td>
          <td>19</td>
          <td>26</td>
          <td>3653</td>
          <td>110</td>
          <td>190</td>
        </tr>
        <tr>
          <th>426</th>
          <td>Volvo</td>
          <td>V40</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$26,135</td>
          <td>$24,641</td>
          <td>1.9</td>
          <td>4.0</td>
          <td>170</td>
          <td>22</td>
          <td>29</td>
          <td>2822</td>
          <td>101</td>
          <td>180</td>
        </tr>
        <tr>
          <th>427</th>
          <td>Volvo</td>
          <td>XC70</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>All</td>
          <td>$35,145</td>
          <td>$33,112</td>
          <td>2.5</td>
          <td>5.0</td>
          <td>208</td>
          <td>20</td>
          <td>27</td>
          <td>3823</td>
          <td>109</td>
          <td>186</td>
        </tr>
      </tbody>
    </table>
    <p>428 rows × 15 columns</p>
    </div>



.. code:: ipython3

    car[~car.Weight>4000,]




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Make</th>
          <th>Model</th>
          <th>Type</th>
          <th>Origin</th>
          <th>DriveTrain</th>
          <th>MSRP</th>
          <th>Invoice</th>
          <th>EngineSize</th>
          <th>Cylinders</th>
          <th>Horsepower</th>
          <th>MPG_City</th>
          <th>MPG_Highway</th>
          <th>Weight</th>
          <th>Wheelbase</th>
          <th>Length</th>
        </tr>
      </thead>
      <tbody>
      </tbody>
    </table>
    </div>



.. code:: ipython3

    car




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Make</th>
          <th>Model</th>
          <th>Type</th>
          <th>Origin</th>
          <th>DriveTrain</th>
          <th>MSRP</th>
          <th>Invoice</th>
          <th>EngineSize</th>
          <th>Cylinders</th>
          <th>Horsepower</th>
          <th>MPG_City</th>
          <th>MPG_Highway</th>
          <th>Weight</th>
          <th>Wheelbase</th>
          <th>Length</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>0</th>
          <td>Acura</td>
          <td>MDX</td>
          <td>SUV</td>
          <td>Asia</td>
          <td>All</td>
          <td>$36,945</td>
          <td>$33,337</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>265</td>
          <td>17</td>
          <td>23</td>
          <td>4451</td>
          <td>106</td>
          <td>189</td>
        </tr>
        <tr>
          <th>1</th>
          <td>Acura</td>
          <td>RSX Type S 2dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$23,820</td>
          <td>$21,761</td>
          <td>2.0</td>
          <td>4.0</td>
          <td>200</td>
          <td>24</td>
          <td>31</td>
          <td>2778</td>
          <td>101</td>
          <td>172</td>
        </tr>
        <tr>
          <th>2</th>
          <td>Acura</td>
          <td>TSX 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$26,990</td>
          <td>$24,647</td>
          <td>2.4</td>
          <td>4.0</td>
          <td>200</td>
          <td>22</td>
          <td>29</td>
          <td>3230</td>
          <td>105</td>
          <td>183</td>
        </tr>
        <tr>
          <th>3</th>
          <td>Acura</td>
          <td>TL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$33,195</td>
          <td>$30,299</td>
          <td>3.2</td>
          <td>6.0</td>
          <td>270</td>
          <td>20</td>
          <td>28</td>
          <td>3575</td>
          <td>108</td>
          <td>186</td>
        </tr>
        <tr>
          <th>4</th>
          <td>Acura</td>
          <td>3.5 RL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$43,755</td>
          <td>$39,014</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>225</td>
          <td>18</td>
          <td>24</td>
          <td>3880</td>
          <td>115</td>
          <td>197</td>
        </tr>
        <tr>
          <th>...</th>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
        </tr>
        <tr>
          <th>423</th>
          <td>Volvo</td>
          <td>C70 LPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$40,565</td>
          <td>$38,203</td>
          <td>2.4</td>
          <td>5.0</td>
          <td>197</td>
          <td>21</td>
          <td>28</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>424</th>
          <td>Volvo</td>
          <td>C70 HPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$42,565</td>
          <td>$40,083</td>
          <td>2.3</td>
          <td>5.0</td>
          <td>242</td>
          <td>20</td>
          <td>26</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>425</th>
          <td>Volvo</td>
          <td>S80 T6 4dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$45,210</td>
          <td>$42,573</td>
          <td>2.9</td>
          <td>6.0</td>
          <td>268</td>
          <td>19</td>
          <td>26</td>
          <td>3653</td>
          <td>110</td>
          <td>190</td>
        </tr>
        <tr>
          <th>426</th>
          <td>Volvo</td>
          <td>V40</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$26,135</td>
          <td>$24,641</td>
          <td>1.9</td>
          <td>4.0</td>
          <td>170</td>
          <td>22</td>
          <td>29</td>
          <td>2822</td>
          <td>101</td>
          <td>180</td>
        </tr>
        <tr>
          <th>427</th>
          <td>Volvo</td>
          <td>XC70</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>All</td>
          <td>$35,145</td>
          <td>$33,112</td>
          <td>2.5</td>
          <td>5.0</td>
          <td>208</td>
          <td>20</td>
          <td>27</td>
          <td>3823</td>
          <td>109</td>
          <td>186</td>
        </tr>
      </tbody>
    </table>
    <p>428 rows × 15 columns</p>
    </div>



.. code:: ipython3

    car[car["Weight"]>4000]




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Make</th>
          <th>Model</th>
          <th>Type</th>
          <th>Origin</th>
          <th>DriveTrain</th>
          <th>MSRP</th>
          <th>Invoice</th>
          <th>EngineSize</th>
          <th>Cylinders</th>
          <th>Horsepower</th>
          <th>MPG_City</th>
          <th>MPG_Highway</th>
          <th>Weight</th>
          <th>Wheelbase</th>
          <th>Length</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>0</th>
          <td>Acura</td>
          <td>MDX</td>
          <td>SUV</td>
          <td>Asia</td>
          <td>All</td>
          <td>$36,945</td>
          <td>$33,337</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>265</td>
          <td>17</td>
          <td>23</td>
          <td>4451</td>
          <td>106</td>
          <td>189</td>
        </tr>
        <tr>
          <th>15</th>
          <td>Audi</td>
          <td>A4 3.0 Quattro convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>All</td>
          <td>$44,240</td>
          <td>$40,075</td>
          <td>3.0</td>
          <td>6.0</td>
          <td>220</td>
          <td>18</td>
          <td>25</td>
          <td>4013</td>
          <td>105</td>
          <td>180</td>
        </tr>
        <tr>
          <th>17</th>
          <td>Audi</td>
          <td>A6 4.2 Quattro 4dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>All</td>
          <td>$49,690</td>
          <td>$44,936</td>
          <td>4.2</td>
          <td>8.0</td>
          <td>300</td>
          <td>17</td>
          <td>24</td>
          <td>4024</td>
          <td>109</td>
          <td>193</td>
        </tr>
        <tr>
          <th>18</th>
          <td>Audi</td>
          <td>A8 L Quattro 4dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>All</td>
          <td>$69,190</td>
          <td>$64,740</td>
          <td>4.2</td>
          <td>8.0</td>
          <td>330</td>
          <td>17</td>
          <td>24</td>
          <td>4399</td>
          <td>121</td>
          <td>204</td>
        </tr>
        <tr>
          <th>20</th>
          <td>Audi</td>
          <td>RS 6 4dr</td>
          <td>Sports</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$84,600</td>
          <td>$76,417</td>
          <td>4.2</td>
          <td>8.0</td>
          <td>450</td>
          <td>15</td>
          <td>22</td>
          <td>4024</td>
          <td>109</td>
          <td>191</td>
        </tr>
        <tr>
          <th>...</th>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
        </tr>
        <tr>
          <th>401</th>
          <td>Volkswagen</td>
          <td>Touareg V6</td>
          <td>SUV</td>
          <td>Europe</td>
          <td>All</td>
          <td>$35,515</td>
          <td>$32,243</td>
          <td>3.2</td>
          <td>6.0</td>
          <td>220</td>
          <td>15</td>
          <td>20</td>
          <td>5086</td>
          <td>112</td>
          <td>187</td>
        </tr>
        <tr>
          <th>411</th>
          <td>Volkswagen</td>
          <td>Phaeton 4dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$65,000</td>
          <td>$59,912</td>
          <td>4.2</td>
          <td>8.0</td>
          <td>335</td>
          <td>16</td>
          <td>22</td>
          <td>5194</td>
          <td>118</td>
          <td>204</td>
        </tr>
        <tr>
          <th>412</th>
          <td>Volkswagen</td>
          <td>Phaeton W12 4dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$75,000</td>
          <td>$69,130</td>
          <td>6.0</td>
          <td>12.0</td>
          <td>420</td>
          <td>12</td>
          <td>19</td>
          <td>5399</td>
          <td>118</td>
          <td>204</td>
        </tr>
        <tr>
          <th>415</th>
          <td>Volkswagen</td>
          <td>Passat W8</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$40,235</td>
          <td>$36,956</td>
          <td>4.0</td>
          <td>8.0</td>
          <td>270</td>
          <td>18</td>
          <td>25</td>
          <td>4067</td>
          <td>106</td>
          <td>184</td>
        </tr>
        <tr>
          <th>416</th>
          <td>Volvo</td>
          <td>XC90 T6</td>
          <td>SUV</td>
          <td>Europe</td>
          <td>All</td>
          <td>$41,250</td>
          <td>$38,851</td>
          <td>2.9</td>
          <td>6.0</td>
          <td>268</td>
          <td>15</td>
          <td>20</td>
          <td>4638</td>
          <td>113</td>
          <td>189</td>
        </tr>
      </tbody>
    </table>
    <p>103 rows × 15 columns</p>
    </div>



.. code:: ipython3

    car[~(car["Weight"]>4000)]




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Make</th>
          <th>Model</th>
          <th>Type</th>
          <th>Origin</th>
          <th>DriveTrain</th>
          <th>MSRP</th>
          <th>Invoice</th>
          <th>EngineSize</th>
          <th>Cylinders</th>
          <th>Horsepower</th>
          <th>MPG_City</th>
          <th>MPG_Highway</th>
          <th>Weight</th>
          <th>Wheelbase</th>
          <th>Length</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>1</th>
          <td>Acura</td>
          <td>RSX Type S 2dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$23,820</td>
          <td>$21,761</td>
          <td>2.0</td>
          <td>4.0</td>
          <td>200</td>
          <td>24</td>
          <td>31</td>
          <td>2778</td>
          <td>101</td>
          <td>172</td>
        </tr>
        <tr>
          <th>2</th>
          <td>Acura</td>
          <td>TSX 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$26,990</td>
          <td>$24,647</td>
          <td>2.4</td>
          <td>4.0</td>
          <td>200</td>
          <td>22</td>
          <td>29</td>
          <td>3230</td>
          <td>105</td>
          <td>183</td>
        </tr>
        <tr>
          <th>3</th>
          <td>Acura</td>
          <td>TL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$33,195</td>
          <td>$30,299</td>
          <td>3.2</td>
          <td>6.0</td>
          <td>270</td>
          <td>20</td>
          <td>28</td>
          <td>3575</td>
          <td>108</td>
          <td>186</td>
        </tr>
        <tr>
          <th>4</th>
          <td>Acura</td>
          <td>3.5 RL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$43,755</td>
          <td>$39,014</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>225</td>
          <td>18</td>
          <td>24</td>
          <td>3880</td>
          <td>115</td>
          <td>197</td>
        </tr>
        <tr>
          <th>5</th>
          <td>Acura</td>
          <td>3.5 RL w/Navigation 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$46,100</td>
          <td>$41,100</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>225</td>
          <td>18</td>
          <td>24</td>
          <td>3893</td>
          <td>115</td>
          <td>197</td>
        </tr>
        <tr>
          <th>...</th>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
        </tr>
        <tr>
          <th>423</th>
          <td>Volvo</td>
          <td>C70 LPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$40,565</td>
          <td>$38,203</td>
          <td>2.4</td>
          <td>5.0</td>
          <td>197</td>
          <td>21</td>
          <td>28</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>424</th>
          <td>Volvo</td>
          <td>C70 HPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$42,565</td>
          <td>$40,083</td>
          <td>2.3</td>
          <td>5.0</td>
          <td>242</td>
          <td>20</td>
          <td>26</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>425</th>
          <td>Volvo</td>
          <td>S80 T6 4dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$45,210</td>
          <td>$42,573</td>
          <td>2.9</td>
          <td>6.0</td>
          <td>268</td>
          <td>19</td>
          <td>26</td>
          <td>3653</td>
          <td>110</td>
          <td>190</td>
        </tr>
        <tr>
          <th>426</th>
          <td>Volvo</td>
          <td>V40</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$26,135</td>
          <td>$24,641</td>
          <td>1.9</td>
          <td>4.0</td>
          <td>170</td>
          <td>22</td>
          <td>29</td>
          <td>2822</td>
          <td>101</td>
          <td>180</td>
        </tr>
        <tr>
          <th>427</th>
          <td>Volvo</td>
          <td>XC70</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>All</td>
          <td>$35,145</td>
          <td>$33,112</td>
          <td>2.5</td>
          <td>5.0</td>
          <td>208</td>
          <td>20</td>
          <td>27</td>
          <td>3823</td>
          <td>109</td>
          <td>186</td>
        </tr>
      </tbody>
    </table>
    <p>325 rows × 15 columns</p>
    </div>



5 instructions (Applying funtion on a column )
==============================================

::

       increase all the values of " MPG_City" column by 3

.. code:: ipython3

    car["MPG_City"]=car["MPG_City"].apply(lambda x:x+3)



.. code:: ipython3

    car




.. raw:: html

    <div>
    <style scoped>
        .dataframe tbody tr th:only-of-type {
            vertical-align: middle;
        }
    
        .dataframe tbody tr th {
            vertical-align: top;
        }
    
        .dataframe thead th {
            text-align: right;
        }
    </style>
    <table border="1" class="dataframe">
      <thead>
        <tr style="text-align: right;">
          <th></th>
          <th>Make</th>
          <th>Model</th>
          <th>Type</th>
          <th>Origin</th>
          <th>DriveTrain</th>
          <th>MSRP</th>
          <th>Invoice</th>
          <th>EngineSize</th>
          <th>Cylinders</th>
          <th>Horsepower</th>
          <th>MPG_City</th>
          <th>MPG_Highway</th>
          <th>Weight</th>
          <th>Wheelbase</th>
          <th>Length</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th>0</th>
          <td>Acura</td>
          <td>MDX</td>
          <td>SUV</td>
          <td>Asia</td>
          <td>All</td>
          <td>$36,945</td>
          <td>$33,337</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>265</td>
          <td>20</td>
          <td>23</td>
          <td>4451</td>
          <td>106</td>
          <td>189</td>
        </tr>
        <tr>
          <th>1</th>
          <td>Acura</td>
          <td>RSX Type S 2dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$23,820</td>
          <td>$21,761</td>
          <td>2.0</td>
          <td>4.0</td>
          <td>200</td>
          <td>27</td>
          <td>31</td>
          <td>2778</td>
          <td>101</td>
          <td>172</td>
        </tr>
        <tr>
          <th>2</th>
          <td>Acura</td>
          <td>TSX 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$26,990</td>
          <td>$24,647</td>
          <td>2.4</td>
          <td>4.0</td>
          <td>200</td>
          <td>25</td>
          <td>29</td>
          <td>3230</td>
          <td>105</td>
          <td>183</td>
        </tr>
        <tr>
          <th>3</th>
          <td>Acura</td>
          <td>TL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$33,195</td>
          <td>$30,299</td>
          <td>3.2</td>
          <td>6.0</td>
          <td>270</td>
          <td>23</td>
          <td>28</td>
          <td>3575</td>
          <td>108</td>
          <td>186</td>
        </tr>
        <tr>
          <th>4</th>
          <td>Acura</td>
          <td>3.5 RL 4dr</td>
          <td>Sedan</td>
          <td>Asia</td>
          <td>Front</td>
          <td>$43,755</td>
          <td>$39,014</td>
          <td>3.5</td>
          <td>6.0</td>
          <td>225</td>
          <td>21</td>
          <td>24</td>
          <td>3880</td>
          <td>115</td>
          <td>197</td>
        </tr>
        <tr>
          <th>...</th>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
          <td>...</td>
        </tr>
        <tr>
          <th>423</th>
          <td>Volvo</td>
          <td>C70 LPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$40,565</td>
          <td>$38,203</td>
          <td>2.4</td>
          <td>5.0</td>
          <td>197</td>
          <td>24</td>
          <td>28</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>424</th>
          <td>Volvo</td>
          <td>C70 HPT convertible 2dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$42,565</td>
          <td>$40,083</td>
          <td>2.3</td>
          <td>5.0</td>
          <td>242</td>
          <td>23</td>
          <td>26</td>
          <td>3450</td>
          <td>105</td>
          <td>186</td>
        </tr>
        <tr>
          <th>425</th>
          <td>Volvo</td>
          <td>S80 T6 4dr</td>
          <td>Sedan</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$45,210</td>
          <td>$42,573</td>
          <td>2.9</td>
          <td>6.0</td>
          <td>268</td>
          <td>22</td>
          <td>26</td>
          <td>3653</td>
          <td>110</td>
          <td>190</td>
        </tr>
        <tr>
          <th>426</th>
          <td>Volvo</td>
          <td>V40</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>Front</td>
          <td>$26,135</td>
          <td>$24,641</td>
          <td>1.9</td>
          <td>4.0</td>
          <td>170</td>
          <td>25</td>
          <td>29</td>
          <td>2822</td>
          <td>101</td>
          <td>180</td>
        </tr>
        <tr>
          <th>427</th>
          <td>Volvo</td>
          <td>XC70</td>
          <td>Wagon</td>
          <td>Europe</td>
          <td>All</td>
          <td>$35,145</td>
          <td>$33,112</td>
          <td>2.5</td>
          <td>5.0</td>
          <td>208</td>
          <td>23</td>
          <td>27</td>
          <td>3823</td>
          <td>109</td>
          <td>186</td>
        </tr>
      </tbody>
    </table>
    <p>428 rows × 15 columns</p>
    </div>



