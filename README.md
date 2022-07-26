# Pie-chart-
## PIE CHART IN R PROGRAMMING ###
#Reading the dataset 
data <-read.csv("piedata.csv")
View(data) #Viewing the dataset


pie(data$amounts)

#Drawing the pie chart with labels 
pie(data$amounts, labels = as.character(data$names))

#You can also change the colors 
pie(data$amounts, labels = as.character(data$names), col = terrain.colors(6))
