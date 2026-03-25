# Revenue Data and Building a Dashboard — Quiz Answers

## Question 2
**What parsers are available in BeautifulSoup for processing HTML content?**

- [x] lxml
- [ ] xml
- [x] html5lib
- [ ] yaml

**Answer:** `lxml` and `html5lib`

---

## Question 3
**What is the advantage of converting the 'Date' column to a datetime data type when analyzing stock data?**

- [ ] It minimizes the size of the dataset
- [ ] It increases computational efficiency
- [ ] It alters the date and time values
- [x] It facilitates accurate plotting of time-series data

**Answer:** `It facilitates accurate plotting of time-series data`

---

## Question 4
**Given the dataset below, select the correct option to remove the `$` symbol and commas from the `Price` column.**

Sample dataset:

| Product  | Quantity | Price     |
|----------|----------|-----------|
| Laptop   | 10       | $1,200.50 |
| Phone    | 25       | $850.00   |
| Tablet   | 15       | $600.75   |
| Monitor  | 8        | $1,050.25 |
| Keyboard | 30       | $120.99   |

Options:

- [ ] `df["Price"] = df["Price"].map(lambda x: x.strip("$,"))`
- [x] `df["Price"] = df["Price"].str.replace(',|\$',"", regex=True)`
- [ ] `df["Price"] = df["Price"].replace("$,", "")`
- [ ] `df["Price"] = df.Price.apply(float)`

**Answer:**
```python
df["Price"] = df["Price"].str.replace(',|\$',"", regex=True)
