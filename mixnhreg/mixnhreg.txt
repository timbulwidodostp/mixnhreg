# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Mixtures of Non-Homogenous Linear Regression Models Use mixnhreg With (In) R Software
install.packages("remotes")
remotes::install_github("jobstdavid/mixnhreg")
library("mixnhreg")
mixnhreg = read.csv("https://raw.githubusercontent.com/timbulwidodostp/mixnhreg/main/mixnhreg/mixnhreg.csv",sep = ";")
# Estimation Mixtures of Non-Homogenous Linear Regression Models Use mixnhreg With (In) R Software
mixnhreg <- mixnhreg(formula = obs ~ sin1 + cos1 + temp_mean | temp_ctrl, scale.formula = ~ sin1 + cos1 + log(temp_sd) | 1, 
weight.formula = ~ sin1 + cos1 | 1, data = mixnhreg, control = control_optim())
summary(mixnhreg)
# Mixtures of Non-Homogenous Linear Regression Models Use mixnhreg With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished