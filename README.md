### PostgreSQL

| Isolation Level    | Dirty Read | Nonrepeatable Read | Phantom Read | Serialization Anomaly | Lost Update |
|---------------------|------------|---------------------|--------------|------------------------|-------------|
| Read uncommitted    | YES        | YES                 | YES          | YES                    | YES         |
| Read committed      | NO         | YES                 | YES          | YES                    | YES         |
| Repeatable read     | NO         | NO                  | NO*          | YES*                   | NO          |
| Serializable        | NO         | NO                  | NO           | NO                     | NO          |

### Percona

| Isolation Level    | Dirty Read | Nonrepeatable Read | Phantom Read | Serialization Anomaly | Lost Update |
|---------------------|------------|---------------------|--------------|------------------------|-------------|
| Read uncommitted    | YES        | YES                 | YES          | YES                    | YES         |
| Read committed      | NO         | YES                 | YES          | YES                    | YES         |
| Repeatable read     | NO         | NO                  | YES*         | NO*                    | NO          |
| Serializable        | NO         | NO                  | NO           | NO                     | NO          |
