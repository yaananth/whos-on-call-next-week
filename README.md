# Who's On Call Next Week?

[![GitHub Actions build badge](https://github.com/github/whos-on-call-next-week/workflows/build-test/badge.svg)](https://github.com/github/whos-on-call-next-week/actions?query=workflow%3Abuild-test)

GitHub Action to look up who's on call next week.

## Example

```yml
- uses: github/whos-on-call-next-week@dev
  with:
    scheduleId: PVHAB95 # actions-service-oncall-primary
    pagerDutyToken: ${{ secrets.PAGERDUTY_API_TOKEN }}
```

## Contributing

### Running tests

```bash
export PAGERDUTY_API_KEY="your PagerDuty API key"
export PAGERDUTY_SCHEDULE_ID="your PagerDuty schedule ID"
npm run test
```