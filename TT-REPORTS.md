## Vybrané reporty pro TT

### Stažení subscription events pro daný den

```bash
./reporter.py -u sarsonj@gmail.com --account 271572 getSubscriptionEventReport 85201870 20230225 -T ${REPORTER_CODE}
```

### Stažení subscription events pro celý měsíc (zde únor)
```bash
for day in {01..28}; do ./reporter.py -u sarsonj@gmail.com --account 271572 getSubscriberReport 85201870 202302${day} -T ${REPORTER_CODE}; done
```

### Grep na počet např. offer codes
```bash
grep -r -c "40 percent off version 1"  Subscriber_*
```