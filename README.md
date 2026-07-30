---
title: "My Leaflet Map"
author: "FL"
date: "2026-07-29"
output: html_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

## Introduction

This map was created in R Markdown using the Leaflet package. 

```{r, echo=FALSE}
library(leaflet)

leaflet() %>%
  addTiles() %>%
  addMarkers(lng = 24.9384, lat = 60.1699, popup = "Helsinki, Finland")
