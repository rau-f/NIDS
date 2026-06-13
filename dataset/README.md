# Dataset: `network_traffic.csv`

A simplified network traffic dataset derived from the well-known NSL-KDD
network intrusion dataset. Each row is a single network connection described
by 15 numeric features plus one binary target column.

- Rows: **6,000** (balanced: 3,000 normal + 3,000 attack)
- Format: CSV, comma separated, with a header row
- All features are already numeric -> **no encoding needed**
- No missing values -> **no imputation needed**

## Target column

| column | meaning                |
| ------ | ---------------------- |
| label  | 0 = normal, 1 = attack |

## Feature columns

| column                 | type | short description                                                   |
| ---------------------- | ---- | ------------------------------------------------------------------- |
| duration               | int  | length (in seconds) of the connection                               |
| src_bytes              | int  | number of data bytes from source to destination                     |
| dst_bytes              | int  | number of data bytes from destination to source                     |
| wrong_fragment         | int  | number of "wrong" fragments in the connection                       |
| hot                    | int  | number of "hot" indicators (e.g. access to sensitive files)         |
| logged_in              | 0/1  | 1 if the user is successfully logged in, 0 otherwise                |
| num_compromised        | int  | number of "compromised" conditions observed                         |
| count                  | int  | connections to the same host in the last 2 seconds                  |
| srv_count              | int  | connections to the same service in the last 2 seconds               |
| serror_rate            | 0..1 | fraction of connections that have SYN errors (host-based)           |
| same_srv_rate          | 0..1 | fraction of connections to the same service                         |
| diff_srv_rate          | 0..1 | fraction of connections to different services                       |
| dst_host_count         | int  | connections to the same destination host                            |
| dst_host_srv_count     | int  | connections to the same destination host and service                |
| dst_host_same_srv_rate | 0..1 | fraction of connections to the same service on the destination host |