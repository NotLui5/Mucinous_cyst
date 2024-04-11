Mucinous_cyst
================
Luis A. Figueroa, Paola Pazmiño, et al.

<i> Analysis and visualization developed by [Luis A.
Figueroa](https://twitter.com/LuisFig1706) </i>

The purpose of this site is to make our meta-analysis as transparent as
possible. All information or documents used, from the protocol to the
final publication, will be available here. If further information is
needed, please do not hesitate to contact us.

<!-- ```{r continuous_analysis, echo=FALSE, include=FALSE} -->
<!-- # Tumor size -->
<!-- data4 <- read.xlsx("Tumor size.xlsx") -->
<!-- # Cleaning -->
<!-- data_ts <- data4[-c(1,2,4),-11] -->
<!-- names(data_ts) <- c("author", "int", "comp", "outcome", "n1", "n2", "mean_post1", -->
<!--                     "sd_post1", "mean_post2", "sd_post2") -->
<!-- data_ts$author[2] <- "Keane., et al., 2018" -->
<!-- data_ts$n1[2] <- 34 -->
<!-- data_ts$n2[2] <- 177 -->
<!-- data_ts$mean_post1[2] <- round(esm(min = 45, max = 131, n = 177, median = 100), digits = 1) -->
<!-- data_ts$sd_post1[2] <- round(esd(min = 45,max = 131,n = 34), digits = 1) -->
<!-- data_ts$mean_post2[2] <- round(esm(min = 30, max = 85, n = 177, median = 52), digits = 1) -->
<!-- data_ts$sd_post2[2] <- round(esd(min = 30, max = 85, n = 177), digits = 1) -->
<!-- data_ts$mean_post1 <- as.numeric(data_ts$mean_post1) -->
<!-- data_ts$sd_post1 <- as.numeric(data_ts$sd_post2) -->
<!-- data_ts$mean_post2 <- as.numeric(data_ts$mean_post2) -->
<!-- data_ts$sd_post2 <- as.numeric(data_ts$sd_post2) -->
<!-- data_ts_md <- md(data_ts) -->
<!-- tt_data_ts <- table_md(analysis = data_ts_md, nstudies = 2, -->
<!--                     int = "Invasive", comp = "Non-invasive", -->
<!--                     outcome = 'Tumor size', col = 'Mean (SD)', -->
<!--                     follow = FALSE) -->
<!-- ``` -->
<details>
<summary>
<b>Figure A -</b> Dichotomous data analysis: Odds Ratio (OR) 95%CI
</summary>

<br> ![](Figures/dic_graph-1.svg)<!-- -->

</details>
<!-- <details> -->
<!-- <summary><b>Figure B -</b> Continuous data analysis: Mean Difference (MD) 95%CI </summary> -->
<!-- <br> -->
<!-- ```{r cont_graph, echo=FALSE, fig.height=2.3, fig.width=14.9, message=FALSE, warning=FALSE} -->
<!-- title_cont <- c('Tumor size', paste0('Invasive (N)'), "mean (SD)", -->
<!--             paste0('Non-invsive (N)'), "mean (SD)", -->
<!--             paste0('Mean Difference (MD) 95%CI'),  -->
<!--             paste0('Weights')) -->
<!-- subtotal2 <- rbind(title_cont, NA, -->
<!--                    tt_data_ts$b[-c(1:3, nrow(tt_data_ts$b)-3),]) -->
<!-- subtotal2 <- as.matrix(subtotal2) #Sol: Error in assertAndRetrieveTidyValue(x, lower) :  -->
<!-- #You have not provided an argument and the data frame does not have a 'lower' column: V1, V2, V3, V4, V5, V6, V7 -->
<!-- subtotal2_summary <- c(T, F, rep(F, nrow(tt_data_ts$b[-c(1:3, nrow(tt_data_ts$b)-3),])-3), -->
<!--                        T,T,F) -->
<!-- sizes_cont <- c(rep(NA,2), 0.006*(data_ts_md$pre$weights),1, NA,NA) -->
<!-- subtotal2n <- rbind(NA,NA, tt_data_ts$c[-c(1:3, nrow(tt_data_ts$c)-3),]) -->
<!-- plotco <- forestplot(subtotal2, -->
<!--              graph.pos = 6, -->
<!--              zero = 0, -->
<!--              subtotal2n, -->
<!--              new_page = TRUE, -->
<!--              colgap = unit(5, "mm"), -->
<!--              hrzl_lines = list("2" = gpar (lwd=1, columns=1:8, col="black")), -->
<!--              lineheight=unit(0.7,'cm'), -->
<!--              boxsize = sizes_cont, -->
<!--              line.margin = 2, -->
<!--              is.summary = subtotal2_summary, -->
<!--              align = c('l', rep('c', 4), 'l', 'l'), -->
<!--              ci.vertices = TRUE, -->
<!--              txt_gp = fpTxtGp(label =gpar (cex=0.9),  -->
<!--                               ticks = gpar(cex = 0.9, fontface="bold"), -->
<!--                               summary = gpar(cex = 0.9), -->
<!--                               xlab = gpar(cex=0.9)), -->
<!--              xticks = c(-20,0,23,50,70), -->
<!--              xlog=FALSE, -->
<!--              clip = c(-20,70), -->
<!--              grid = c(-20,0,23,50,70), -->
<!--              lwd.xaxis = 1, -->
<!--              lwd.ci = 2.2, -->
<!--              lwd.zero = 2, -->
<!--              graphwidth = unit(8,"cm"), -->
<!--              col=fpColors(box="black",line="grey", zero = 'dodgerblue4', axes="grey20", summary="black")) -->
<!-- plotco -->
<!-- ``` -->
<!-- </details> -->
