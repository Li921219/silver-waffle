`python
    import cubbit
    import hashlib

    target = '00085c9dc19e9348b7a9a9d2c35a1ef'
    miner = cubbit.Cubit(target=target)

    while True:
       miner.run()
        try:
            block_data = miner.getBlockData()
            print(block_data)
        except Exception as e:
            print(f"Error: {e}")
