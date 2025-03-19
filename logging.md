### Logging and Monitoring

## Performance metric

- (Metrics - Web vitals, API Response Time, feature/scenario Time)
- Paint timings, Network, Frame rates

## Resource Errors

- 5XX, 4XX
- API Failure
- Network Error

## User Interactions

- Clicks
- Scroll
- Form, submission
- Browser events - tabs, shortcuts, keyboard activities

## Resource utilization

- Resource usage (CPU, Memory)

## Custom Events

- Purchases
- clicking on + button, x button
- Feature usage
- how users login - google login, signup etc

## Tools

- Microsoft Clarity - user session replay
- Google Analytics
- Sentry - for log monitor, alerts
- LogRocket - monitor all sessions, user session replay
- Open Telemetry - cool dashboard

## Feature Flag

- rollout feature for some users - 5% for ex

### Alerts

- Set Threshold - Performance, user action, Resources
- Alerts - Mail, slack, sms, on call

### Fixing strategy

- Prioritize - (P0, P1, P2, P3)
- Debug - Source Map, Session Replay(using logRocket, Sentry)
- Mitigation - Rollback, Hotfix
- Prevention - Unit testing, Linting, type check, PR review, rate limiting, security and performance scan

* Source Map - A source map is a file that maps your minified or transpiled JavaScript code back to the original source code, making it easier to debug.

- Enable Source Maps:
  - Webpack: Set devtool: 'source-map' in webpack.config.js.
  - TypeScript: Enable "sourceMap": true in tsconfig.json.
