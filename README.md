# aws-security-group-action

```
    steps:
      - id: open-firewall
        uses: kowsheek/aws-security-group-action@v1.0.0
        with:
          group-id: 'sg-XXXXXX'
          aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
          aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
          aws-region: 'us-east-1'
          action: 'open'
          
      - id: close-firewall
        uses: kowsheek/aws-security-group-action@v1
        with:
          group-id: 'sg-XXXXXX'
          aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
          aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
          aws-region: 'us-east-1'
          action: 'close'
      
```
