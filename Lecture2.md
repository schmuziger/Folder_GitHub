# Lecture 2

# Create numeric vector
Freedom_press <- c(90, 80, 50, 60, 95, 88, 77, 55)

# Create character vector
Countries <- c('Argentina', 'Brazil', 'Venezuela', "Bolivia", "Chile", "Uruguay", "Mexico", "Cuba")

# Create numeric vector
PolSys <- c(1, 1, 2, 1, 1, 1, 1, 2)

# Create character vector for factor labels
Regimes <- c('democracy', 'autocracy')

# Convert to labelled factor
CountryRegime_factor <- factor(PolSys, labels = Regimes)

summary(CountryRegime_factor)

combined <- cbind(Freedom_press, Countries, PolSys, CountryRegime_factor)

# Combine numeric_vector and character_vector into a data frame

combined_df1 <- data.frame(Freedom_press, Countries, PolSys, CountryRegime_factor, stringsAsFactors = FALSE)

combined_df1

hist(combined_df1$Freedom_press)

View(combined_df1)

###################################

numeric_vector <- c(1, 2, 3)
character_vector <- c("A", "B", "C")
logical_vector <- c()
factor_vector <- c()