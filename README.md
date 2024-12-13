# MedianImputer
# create variable
item <- c("cups", "plates", "burgers", "buns", "forks", "ketchups")
quantity <- c(46, NA, 100, 80, 60, 30)
month <- c(2,3,4,3,7,NA)
day <- c(14, 02, NA, 16, 24, 01)
# create dataset
orders <- data.frame(item, quantity, month, day)
#display dataset
orders

# Function to perform imputation for missing values
#' Title
#'
#' @param orders
#'
#' @return
#' @export
#'
#' @examples
orders_imputed <- function(orders) {
  # Iterate through each column in the datasets
  for (i in i:ncol(orders_imputed)) {
    # Check if the column is numeric
    if (is.numeric(orders_imputed[[i]])) {
      # Calculate the median excluding NA values
      median_value <- median(data[[col]], na.rm = TRUE)

      # Replace NA values with the median
      orders_imputed[[i]][is.na(orders_imputed[[i]])] <- median_value
    }
  }

  # Return the modified datasets
  return(orders_imputed)
}

summarry(orders_imputed)

# 'name(Orders_MedianImputed)
# 'This function is about orders with missing values in it
# 'function (x)
# 'x is from the name ofyour datasets
# 'authors("Khalifa Halim")
# 'function (orders)
