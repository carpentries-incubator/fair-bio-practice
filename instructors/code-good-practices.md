## Coding Good Practices
Before we let you go wild in our subsequent exercises we would like to go highlight a
few standards and best practices that will help you generate cleaner, more readable, 
more efficient code. (Note: this code is an example for coding in R, but best practices
apply to any code)

### Advantages of using Coding Standards
* ability to retrace code created by different programmers (uniformity)
* reusable code
* easier to detect errors
* code is simpler, more readable, easier to maintain
* allows to generate faster results and work more efficiently

### Best Practices
* write as few lines as possible (this will make your code faster)
* use appropriate names to describe your variables: e.g. df for dataframe instead of x
* segment blocks of code in the same section into paragraphs e.g. note the difference below following two code blocks

```
## Wrong
library(ggplot2)
df <- read.delim(file = "light_results.txt")
df
df$genotype <- factor(df$genotype, levels = c("WT", "PhyA-211","elf4-101"))
options(repr.plot.width = 5, repr.plot.height = 4)
ggplot(subset(df, light_condition %in% "SD"),
       mapping = aes(x = genotype, y = biomas, fill = genotype)) +
    geom_boxplot() +
    labs(title = "Biomas per Genotype on short days",
        x = "Genotype",
        y = "Biomas (g)") +
    scale_fill_manual(values=c("#999999", "#E69F00", "#56B4E9"))
```  

```
## Better
df <- read.delim(file = "light_results.txt")
df

df$genotype <- factor(df$genotype, levels = c("WT", "PhyA-211","elf4-101"))

options(repr.plot.width = 5, repr.plot.height = 4)
ggplot(subset(df, light_condition %in% "SD"),
       mapping = aes(x = genotype, y = biomas, fill = genotype)) +
    geom_boxplot() +
    labs(title = "Biomas per Genotype on short days",
        x = "Genotype",
        y = "Biomas (g)") +
    scale_fill_manual(values=c("#999999", "#E69F00", "#56B4E9"))
```
* use indentations to mark the beginning and end of structures: note the difference in 
the two code blocks below. The indentations clearly mark that mapping belongs within 
the function of ggplot, x and y clearly belong to labs. The other functions are being 
passed to the ggplot function and allow to change overall plot appearance.

```
## Wrong
ggplot(subset(df, light_condition %in% "SD"),
mapping = aes(x = genotype, y = biomas, fill = genotype)) +
geom_boxplot() +
labs(title = "Biomas per Genotype on short days",
x = "Genotype",
y = "Biomas (g)") +
scale_fill_manual(values=c("#999999", "#E69F00", "#56B4E9"))
```

```
## Better
ggplot(subset(df, light_condition %in% "SD"),
       mapping = aes(x = genotype, y = biomas, fill = genotype)) +
    geom_boxplot() +
    labs(title = "Biomas per Genotype on short days",
        x = "Genotype",
        y = "Biomas (g)") +
    scale_fill_manual(values=c("#999999", "#E69F00", "#56B4E9"))
```
* Whilst indentations are great, don't go too deep, as this will make code harder to 
read and follow.
* Don't repeat yourself!! If there is a repetitive task, automate this using a function 
or already existing packages (R and Python have many data wrangling packages available)
* Avoid long lines: horizontal block text is easier to read for us humans. Note the 
difference between these two code blocks

```
## Wrong
ggplot(subset(df, light_condition %in% "SD"), mapping = aes(x = genotype, y = biomas, fill = genotype)) + geom_boxplot() + labs(title = "Biomas per Genotype on short days", x = "Genotype", y = "Biomas (g)") + scale_fill_manual(values=c("#999999", "#E69F00", "#56B4E9"))
```

```
## Better
ggplot(subset(df, light_condition %in% "SD"),
       mapping = aes(x = genotype, y = biomas, fill = genotype)) +
    geom_boxplot() +
    labs(title = "Biomas per Genotype on short days",
        x = "Genotype",
        y = "Biomas (g)") +
    scale_fill_manual(values=c("#999999", "#E69F00", "#56B4E9"))
```

* most importantly leave comments of what your code does! Describe code functions
throughout, add headers in between analysis steps (if code is self-explanatory this is not
necessary - e.g. in our lesson we annotated all code as not everyone is familiar with R)

```
## Ideal

## plot the graph using ggplot
ggplot(subset(df, light_condition %in% "SD"), # subset only SD from light condition column
       mapping = aes(x = genotype, y = biomas, fill = genotype)) + # colours are by genotype
    geom_boxplot() +
    labs(title = "Biomas per Genotype on short days", # define plot title, and x- and y-axis
        x = "Genotype",
        y = "Biomas (g)") +
    scale_fill_manual(values=c("#999999", "#E69F00", "#56B4E9")) # change colour of groups
```

> ## Attribution
> * [Coding Standards best practices](https://www.browserstack.com/guide/coding-standards-best-practices)
{: .callout}


