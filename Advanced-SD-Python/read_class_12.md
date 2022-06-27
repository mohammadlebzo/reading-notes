# Read: Class 12

## Pandas

### Some Pandas concepts and examples:

In order to use pandas, first we need to import **numpy** and **pandas**.

    import numpy as np
    import pandas as pd

### Some ways of object creation using pandas

- Using **series**

        Input:
        pd.series([1., 2., 3.])
        
        Output:
        0   1.0
        1   2.0
        2   3.0
        dtype: float64

- Using **date_range**

        Input:
        pd.date_range("20150101", periods=6)

        Output:
        DatetimeIndex(['2015-01-01', '2015-01-02', '2015-01-03', '2015-01-04', '2015-01-05', '2015-01-06'],
        dtype='datetime64[ns]', freq='D')

- Using **DataFrame** with a dictionary

        Input:
        pd.DataFrame(
            {
                "A": 1.0,
                "B": pd.Timestamp("20150102"),
                "C": pd.Series(1, index=list(range(4)), dtype="float32"),
                "D": np.array([3] * 4, dtype="int32"),
                "E": pd.Categorical(["test", "train", "test", "train"]),
                "F": "deal",
            }
        )

        Output:
            A          B    C   D      E    F
        0  1.0 2013-01-02  1.0  3   test  foo
        1  1.0 2013-01-02  1.0  3  train  foo
        2  1.0 2013-01-02  1.0  3   test  foo
        3  1.0 2013-01-02  1.0  3  train  foo

### Some ways of viewing data using pandas [Data source](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html#viewing-data)

- Viewing the **top** and **bottom** *rows* of a **frame**: 

        Input:
        {series or a DataFrame}.head()
        {series or a DataFrame}.tail(3)

        Output:
                        A         B         C         D
        2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
        2013-01-02  1.212112 -0.173215  0.119209 -1.044236
        2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
        2013-01-04  0.721555 -0.706771 -1.039575  0.271860
        2013-01-05 -0.424972  0.567020  0.276232 -1.087401

                        A         B         C         D
        2013-01-04  0.721555 -0.706771 -1.039575  0.271860
        2013-01-05 -0.424972  0.567020  0.276232 -1.087401
        2013-01-06 -0.673690  0.113648 -1.478427  0.524988

- Converting to a numpy array:

        Input:
        {series or a DataFrame}.to_numpy()

        Output:
        array([[ 0.4691, -0.2829, -1.5091, -1.1356],
                [ 1.2121, -0.1732,  0.1192, -1.0442],
                [-0.8618, -2.1046, -0.4949,  1.0718],
                [ 0.7216, -0.7068, -1.0396,  0.2719],
                [-0.425 ,  0.567 ,  0.2762, -1.0874],
                [-0.6737,  0.1136, -1.4784,  0.525 ]])

- Sorting by a column:

        Input:
        {series or a DataFrame}.sort_values(by="B")

        Output:
                           A         B         C         D
        2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
        2013-01-04  0.721555 -0.706771 -1.039575  0.271860
        2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
        2013-01-02  1.212112 -0.173215  0.119209 -1.044236
        2013-01-06 -0.673690  0.113648 -1.478427  0.524988
        2013-01-05 -0.424972  0.567020  0.276232 -1.087401

### Some ways of selecting data: [Data Source](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html#viewing-data)

- Getting data:

        Input:
        {series or a DataFrame}.["A"]

        Output:
        2013-01-01    0.469112
        2013-01-02    1.212112
        2013-01-03   -0.861849
        2013-01-04    0.721555
        2013-01-05   -0.424972
        2013-01-06   -0.673690
        Freq: D, Name: A, dtype: float64

- Selecting data by it's lable:

        Input:
        {series or a DataFrame}.loc[dates[0]]

        output:
        A    0.469112
        B   -0.282863
        C   -1.509059
        D   -1.135632
        Name: 2013-01-01 00:00:00, dtype: float64

- Selecting data by it's position:

        Input:
        {series or a DataFrame}.iloc[3]

        Output:
        A    0.721555
        B   -0.706771
        C   -1.039575
        D    0.271860
        Name: 2013-01-04 00:00:00, dtype: float64

### Some useful methods that are worth mentioning

|**Method**|**Use**|
|----------|-------|
|mean()|returns the mean of each column|
|apply()|allows you to apply functions to data|
|str.lower|a string method that makes all data lower case|
|concat() and join()|allows you to merge data|

## Things I want to know more about

- None.