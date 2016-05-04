# data_science_with_r_notes
Notes from Hadley Wickham's talk at ACM on May 3, 2016

## Data Science with R

### Hadley Wickham
------------

# little bunny foo foo

foo_foo <- little_bunny()

bop_on(
  scooop_up(
    hop_through(foo_foo_ forest),
    field_mouse
      ),
    head
)

foo_foo %>%
hop_through(forest) %>%
scoop_up(field_mouse) %>%
bop_on(head)

can also use the . as a pronoun e.g.:

`x %>% f(y, .)`

`# f(y, x)`

# The data analysis pipeline

There are seven steps to data analysis (taking data in, knowledge out)
after collection:
import -> tidy -> transform -> visualize -> model -> communicate

not just the verbs matter, but also the arrows. pipes are the glue that binds these parts together.

# Tidy
## consistent way of storing data

|storage|meaning|
|-------|-------|
|column| variable|
|row| observation|
|data.frame|dataset|


`gather()` pulls columns together into a single variable

spread vs. gather

`separate()` splits a variable

extract/separate vs. unite

*to learn more google for:*  google for "tidyr" or "tidydata"

# Transform
## create  new variables and new summaries

venn diagram

(cognitive) (computational)

(Think it( Describe it *precisely*) Calculate it)

tbls do less than data frames, but do the *right* less

e.g. no partial matching on var names

`select` operates on columns

`filter` operates on rows1

`mutate` lets you make new columns (variables)

`arrange` does ordering

`summarise` lets you collapse data

## Joins

### mutating joins:
* inner_join
* left-join
* right-join
* outer

### filtering joins:

* semi - all values of x that match in y
* anti_join - all values of x that do not match in y

`dplyr` translates R into `SQL`

*to learn more google for:* "dplyr"

# Visualize
## surprises, but doesn't scale

`ggvis` is  *grammar*-based, *reactive*, and *of the web*

*to learn more google for:* "ggvis"

ggplot

# Model
## scales, but doesn't (fundamentally) surprise
every model by its nature makes assumptions, but it cannot question those assumptions

# Communicate

## get insights out of your head and into someone else's

*to learn more google for:* Rmarkdown


# Future steps

Create a *pit* of success. Rather than a pinnacle that has to be surmounted, it would be better to have something you can accidentally fall into, that will lead you to success.

You should be able to think about data analysis and your fingers will automatically do the typing.

In the age of google, if you have the name of something you have power over it. If you don't have the name, things become much more difficult.
