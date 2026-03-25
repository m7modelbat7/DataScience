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


## Question 5
**Determine the `Revenue` figure found in the final entry of the `tesla_revenue` dataset.**

- [ ] 30
- [ ] 22
- [ ] 45
- [x] 27

**Answer:** `27`

---

## Question 6
**Select the `Close` value for the first record (dated 2002-02-13) in the extracted GameStop stock data.**

- [ ] 1.693353
- [ ] 1.620128
- [x] 1.691667
- [ ] 1.620396

**Answer:** `1.691667`

---

## Question 7
**Following the graph shown below, which of the following statements best describes the trend in Tesla's stock price and revenue between 2018 and 2021?**

- [x] Both Tesla’s revenue and stock price showed strong growth.
- [ ] Tesla’s stock price increased sharply, but revenue declined.
- [ ] Tesla’s revenue remained flat while stock price dropped significantly.
- [ ] Revenue growth was high, but the stock price stayed constant.

**Answer:** `Both Tesla’s revenue and stock price showed strong growth.`

---

## Question 8
**Following the graph shown below, what key observation can be made about GameStop's stock price and revenue?**

- [ ] Both revenue and stock price followed the same upward trend steadily.
- [x] Stock price surged sharply around 2021, but revenue did not show a similar increase.
- [ ] Stock price and revenue remained stable throughout the timeline.
- [ ] Revenue growth directly caused the stock price surge.

**Answer:** `Stock price surged sharply around 2021, but revenue did not show a similar increase.`
