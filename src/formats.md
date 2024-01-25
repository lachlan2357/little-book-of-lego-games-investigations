# Formats

Throughout this book, different things may require different formats, such as times, dates, time-zones to things like measurements, etc. They may be unclear or ambiguous to different readers depending on their knowledge, country, etc.

## Metric by Default

Like much of the world, and myself in Australia, metric is default, and has been used by default throughout this book. Any measurements that may have conflicting representations are always stated in their metric equivalents (i.e., metres instead of feet, celsius instead of fahrenheit, etc.)

## Time and Date

There are a lot of ways to represent dates, however this book represents them in the `ISO 8601` format, usually meaning the following:

- dates by themselves are represented as `YYYY-MM-DD` with either the `-DD` or `-MM-DD` parts being optional
- times are represented in 24-hours time as `HH:MM:SS.XXX` as hours, minutes, seconds and milliseconds to three decimal places (usually, seconds and milliseconds aren't required)
- time-zones are written as `GMT[s][H]`, e.g., in Brisbane, QLD (Australia) I am `GMT+10` but some are `GMT-8` in the Sacramento, CA (United States of America)