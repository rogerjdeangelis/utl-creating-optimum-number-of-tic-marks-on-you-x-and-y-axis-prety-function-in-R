# utl-creating-optimum-number-of-tic-marks-on-you-x-and-y-axis-prety-function-in-R
Creating optimum number of tic marks on you x and y axis prety function in R
    Creating optimum number of tic marks on you x and y axis prety function in R                                                   
                                                                                                                                   
    github                                                                                                                         
    https://tinyurl.com/ybvjzrsq                                                                                                   
    https://github.com/rogerjdeangelis/utl-creating-optimum-number-of-tic-marks-on-you-x-and-y-axis-prety-function-in-R            
                                                                                                                                   
    R prety function                                                                                                               
    https://stat.ethz.ch/R-manual/R-patched/library/base/html/pretty.html                                                          
                                                                                                                                   
    Tnis function will try to honor the number of intervals you select but will often add or                                       
    subtract intervals to make a 'prettier' spacing.                                                                               
                                                                                                                                   
    https://stackoverflow.com/questions/62491568/understanding-pretty-in-r                                                         
                                                                                                                                   
    *_                   _                                                                                                         
    (_)_ __  _ __  _   _| |_                                                                                                       
    | | '_ \| '_ \| | | | __|                                                                                                      
    | | | | | |_) | |_| | |_                                                                                                       
    |_|_| |_| .__/ \__,_|\__|                                                                                                      
            |_|                                                                                                                    
    ;                                                                                                                              
                                                                                                                                   
                                                                                                                                   
    options validvarname=upcase;                                                                                                   
    libname sd1 "d:/sd1";                                                                                                          
    data sd1.have;                                                                                                                 
      set sashelp.class(keep=height weight);;                                                                                      
      weight=weight/150;                                                                                                           
    run;quit;                                                                                                                      
                                                                                                                                   
                                                                                                                                   
    SD1.HAVE total obs=19                                                                                                          
                                                                                                                                   
      HEIGHT     WEIGHT                                                                                                            
                                                                                                                                   
       51.3     0.33667                                                                                                            
       56.3     0.51333                                                                                                            
       56.5     0.56000                                                                                                            
       57.3     0.55333                                                                                                            
       57.5     0.56667                                                                                                            
       59.0     0.66333                                                                                                            
       59.8     0.56333                                                                                                            
       62.5     0.75000                                                                                                            
       62.5     0.56000                                                                                                            
       62.8     0.68333                                                                                                            
       63.5     0.68333                                                                                                            
       64.3     0.60000                                                                                                            
       64.8     0.85333                                                                                                            
       65.3     0.65333                                                                                                            
       66.5     0.74667                                                                                                            
       66.5     0.74667                                                                                                            
       67.0     0.88667                                                                                                            
       69.0     0.75000                                                                                                            
       72.0     1.00000                                                                                                            
                                                                                                                                   
    *            _               _                                                                                                 
      ___  _   _| |_ _ __  _   _| |_                                                                                               
     / _ \| | | | __| '_ \| | | | __|                                                                                              
    | (_) | |_| | |_| |_) | |_| | |_                                                                                               
     \___/ \__,_|\__| .__/ \__,_|\__|                                                                                              
                    |_|                                                                                                            
    ;                                                                                                                              
              X AXIS                YAXIS                                                                                          
           HEIGHT TICMARKS      WEIGHT TICMARKS                                                                                    
          ================    ==============================                                                                       
    FROMR=50 55 60 65 70 75 @ 0.3 0.4 0.5 0.6 0.7 0.8 0.9 1                                                                        
                                                                                                                                   
                                                                                                                                   
      WEIGHT                                                                                                                       
           50    55    60    65    70    75                                                                                        
          --+-----+-----+-----+-----+-----+---                                                                                     
          |                                  |                                                                                     
      1.0 +                           *      + 1.0                                                                                 
          |                                  |                                                                                     
          |                                  |                                                                                     
      0.9 +                     *            + 0.9                                                                                 
          |                   *              |                                                                                     
          |                                  |                                                                                     
      0.8 +                                  + 0.8                                                                                 
          |                *       *         |                                                                                     
          |                     *            |                                                                                     
      0.7 +                **                + 0.7                                                                                 
          |            *      *              |                                                                                     
          |                                  |                                                                                     
      0.6 +                  *               + 0.6                                                                                 
          |         **  *  *                 |                                                                                     
          |                                  |                                                                                     
      0.5 +         *                        + 0.5                                                                                 
          |                                  |                                                                                     
          |                                  |                                                                                     
      0.4 +                                  + 0.4                                                                                 
          |                                  |                                                                                     
          |   *                              |                                                                                     
      0.3 +                                  + 0.3                                                                                 
          |                                  |                                                                                     
          --+-----+-----+-----+-----+-----+---                                                                                     
           50    55    60    65    70    75                                                                                        
                                                                                                                                   
                         HEIGHT                                                                                                    
    *                    _       __             _ _                                                                                
     ___  __ _ ___    __| | ___ / _| __ _ _   _| | |_                                                                              
    / __|/ _` / __|  / _` |/ _ \ |_ / _` | | | | | __|                                                                             
    \__ \ (_| \__ \ | (_| |  __/  _| (_| | |_| | | |_                                                                              
    |___/\__,_|___/  \__,_|\___|_|  \__,_|\__,_|_|\__|                                                                             
                                                                                                                                   
    ;                                                                                                                              
                                                                                                                                   
    WEIGHT                                                                                                                         
         50         60         70         80                                                                                       
         -+----------+----------+----------+-                                                                                      
         |                                  |                                                                                      
         |                                  |                                                                                      
     1.0 +                        *         + 1.0                                                                                  
         |                                  |                                                                                      
         |                                  |                                                                                      
         |                   *              |                                                                                      
         |                *                 |                                                                                      
     0.8 +                                  + 0.8                                                                                  
         |              *   *  *            |                                                                                      
         |                                  |                                                                                      
         |          *   **                  |                                                                                      
         |                 *                |                                                                                      
     0.6 +                *                 + 0.6                                                                                  
         |       **  *  *                   |                                                                                      
         |       *                          |                                                                                      
         |                                  |                                                                                      
         |                                  |                                                                                      
     0.4 +                                  + 0.4                                                                                  
         |                                  |                                                                                      
         | *                                |                                                                                      
         |                                  |                                                                                      
         |                                  |                                                                                      
     0.2 +                                  + 0.2                                                                                  
         |                                  |                                                                                      
         -+----------+----------+----------+-                                                                                      
         50         60         70         80                                                                                       
                                                                                                                                   
                        HEIGHT                                                                                                     
    *                                                                                                                              
     _ __  _ __ ___   ___ ___  ___ ___                                                                                             
    | '_ \| '__/ _ \ / __/ _ \/ __/ __|                                                                                            
    | |_) | | | (_) | (_|  __/\__ \__ \                                                                                            
    | .__/|_|  \___/ \___\___||___/___/                                                                                            
    |_|                                                                                                                            
    ;                                                                                                                              
                                                                                                                                   
    %symdel fromr / nowarn;                                                                                                        
                                                                                                                                   
    %utl_submit_r64('                                                                                                              
    library(haven);                                                                                                                
    library(SASxport);                                                                                                             
    have<-read_sas("d:/sd1/have.sas7bdat");                                                                                        
    yax<-pretty(have$WEIGHT,5);                                                                                                    
    xax<-pretty(have$HEIGHT,7);                                                                                                    
    xes<-as.character(paste(xax, collapse = " "));                                                                                 
    yes<-as.character(paste(yax, collapse = " "));                                                                                 
    axs<-paste(xes,yes,sep="@");                                                                                                   
    writeClipboard(axs);                                                                                                           
    ',returnvar=fromr);                                                                                                            
                                                                                                                                   
    %put &=fromr;                                                                                                                  
                                                                                                                                   
    FROMR=50 55 60 65 70 75@0.3 0.4 0.5 0.6 0.7 0.8 0.9 1                                                                          
                                                                                                                                   
    option ls=64 ps=33;                                                                                                            
    proc plot data=sd1.have(rename=weight=weight_12345678901234567890);                                                            
      plot weight_12345678901234567890*height='*' / box                                                                            
        haxis=%scan(&fromr,1,"@")                                                                                                  
        vaxis=%scan(&fromr,2,"@") ;                                                                                                
    run;quit;                                                                                                                      
                                                                                                                                   
    * sas default;                                                                                                                 
    option ls=64 ps=33;                                                                                                            
    proc plot data=sd1.have(rename=weight=weight_12345678901234567890);                                                            
      plot weight_12345678901234567890*height='*' / box;                                                                           
    run;quit;                                                                                                                      
                                                                                                                                   
