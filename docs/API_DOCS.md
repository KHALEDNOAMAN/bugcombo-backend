# DebugDuel API Reference

## Authentication
```
POST /api/auth/login
POST /api/auth/register
Authorization: Bearer <token>
```

## Endpoints
### Challenges
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/challenges | List active challenges |
| POST | /api/challenges | Create challenge |
| GET | /api/challenges/:id | Get challenge details |
| POST | /api/challenges/:id/submit | Submit bug fix |

### Duels
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/duels/match | Find opponent |
| GET | /api/duels/:id | Duel status |
| POST | /api/duels/:id/ready | Mark ready |

### Leaderboard
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/leaderboard | Global rankings |
| GET | /api/leaderboard/weekly | Weekly rankings |

## AI Judging
Bug fixes are scored on: correctness, performance, code quality, and time.
