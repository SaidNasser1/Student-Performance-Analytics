BEGIN
    SET threshold = 40
    FOR EACH mark IN studentMarksList:
        IF mark >= threshold:
            passCount = passCount + 1
END
