1.)

    Run 1 locally: exactF2
    Output:
            Exact F2. Time elapsed:128s. Estimate: 8567966130
    ---------------------------
    Run 1 in GCP: BJKST 8 1000
    Arguments:
              gs://brownalu-csci3390-bucket/2014to2017.csv
              exactF2
    Output:
            Exact F2. Time elapsed:60s. Estimate: 8567966130


2.)

    Run 1 Locally: ToW 1 1
    Output:
            Tug-of-War F2 Approximation. Width :1. Depth: 1. Time elapsed:43s. Estimate: 122500
    ---------------------------
    Run 1 in GCP:
    Arguments:
              gs://brownalu-csci3390-bucket/2014to2017.csv
              ToW
              1
              1
    Output:
            Tug-of-War F2 Approximation. Width :1. Depth: 1. Time elapsed:35s. Estimate: 3331367524


    Run 2 in GCP:
    Arguments:
              gs://brownalu-csci3390-bucket/2014to2017.csv
              ToW
              4
              3
    Output:
            Tug-of-War F2 Approximation. Width :4. Depth: 3. Time elapsed:80s. Estimate: 5330439739

    Run 3 in GCP:
    Arguments:
                gs://brownalu-csci3390-bucket/2014to2017.csv
                ToW
                10
                12

    Output:
            Tug-of-War F2 Approximation. Width :10. Depth: 12. Time elapsed:449s. Estimate: 9051723106


3.)

    Run 1 locally: BJKST 8 10000
    Output:
            n/a : took over 30 minutes

    Run 2 locally: BJKST 2 5
    Output:
            BJKST Algorithm. Bucket Size:2. Trials:5. Time elapsed:151s. Estimate: 1.6777216E7
    -----------------------------------
    Run 1 in GCP:
    Arguments:
              gs://brownalu-csci3390-bucket/2014to2017.csv
              BJKST
              8
              1000
    Output:
            n/a : took over 30 minutes


    Run 2 in GCP:
    Arguments:
              gs://brownalu-csci3390-bucket/2014to2017.csv
              BJKST
              2
              10

    Output:
            BJKST Algorithm. Bucket Size:2. Trials:10. Time elapsed:135s. Estimate: 1.6777216E7

    Run 3 in GCP:
    Arguments:
              gs://brownalu-csci3390-bucket/2014to2017.csv
              BJKST
              5
              5

    Output:
            BJKST Algorithm. Bucket Size:5. Trials:5. Time elapsed:71s. Estimate: 3.3554432E7





4.)
      Running exactF0, we get: Exact F0. Time elapsed:97s. Estimate: 7406649
      We can compare this value to BJKST estimate of 1.6777216E7. Exact F0 seems like a valuable
      algorithm for a speedy and accurate estimate while BJKST for more intensive results.

      Running exactF2, we got: Exact F2. Time elapsed:128s. Estimate: 8567966130
      We can compare this value to ToW estimate of 5330439739-9051723106.
      While the speed of the calculation of exactF2 was rather slow, it seems to yield very accurate results given strong computing power.
