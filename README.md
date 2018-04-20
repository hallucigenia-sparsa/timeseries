README

The full-length test time series generated with different models or taken from stool data are in timeseries.zip, versions of these time series with Poisson and multinomial noise are in Poisson.zip and Multinomial.zip, respectively. Stool data are not contained in these two zip files.  

Most time series are raw, i.e. as generated by the models without further processing steps. For the stool time series, data were processed by rarefaction to 10000 reads per sample and interpolated with method "stineman" in the stinepack R package.   

For the Poisson time series, values were sampled from a Poisson distribution that took the original value as a parameter. Prior to Poisson sampling, time series were scaled to a minimum of 1000 counts per sample. For the multinomial time series, samples were generated with the multinomial distribution, given the taxon proportions in each sample. Sequencing depth was varied between 1000 and 1500 with the uniform distribution. 

Time series are stored as tab-delimited tables where rows represent species and columns time points. 
