# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Plotting clustered trees Use clustree With (In) R Software
# Clustered tree plots Use clustree With (In) R Software
# Visualise Clusterings at Different Resolutions Use clustree With (In) R Software
install.packages("readxl")
install.packages("httr")
install.packages("clustree")
install.packages("ggplot2")
library("readxl")
library("httr")
library("ggplot2")
library("clustree")
# Import Data Excel Into R From Github Olah Data Semarang (timbulwidodostp)
github_link <- "https://github.com/timbulwidodostp/clustree/raw/main/clustree/clustree.xlsx"
temp_file <- tempfile(fileext = ".xlsx")
req <- GET(github_link, 
# authenticate using GITHUB_PAT
authenticate(Sys.getenv("GITHUB_PAT"), ""),
# write result to disk
write_disk(path = temp_file))
clustree <- readxl::read_excel(temp_file)
# Estimate Plotting clustered trees Use clustree With (In) R Software
clustree<-clustree(clustree,prefix="K")
clustree
# Plotting clustered trees Use clustree With (In) R Software
# Clustered tree plots Use clustree With (In) R Software
# Visualise Clusterings at Different Resolutions Use clustree With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished