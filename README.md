refactor TO-DO:

1. move constants to consts.js
    - width
        - width of the field
    - height
        - height of the field
    - tileSizes
        - a field has a tile size.
    - maxGrowth
        - max growth tick for a field
    - growthBasePrice
    - speedBasePrice
    - sizeBasePrice
    - tileBasePrice
    - tickBasePrice
    - growthRateMultiplier
    - tickBaseMultiplier
    - mowerRateMultiplier
    - mowerSizeMultiplier
    - tileSizeMultiplier
    - currentlyPrestiging
2. move hardcoded values to consts.js
3. follow MVC pattern
    - models:
        - Upgrade
        - Field
        - Area
    - views:
        - lawn (interacts with canvas and ctx)
        - upgrade texts (responsible for updating cost for upgrade and current stats)
        - prestige (update mulch counter, cost to prestige, current value bonus, growth bonus)
        - others like desc, money, totalMowed, superTicks, and updating unlockNext button
    - controller:
        - one controller that sets up models and views
