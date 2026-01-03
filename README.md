BEGIN
    SET threshold = 50
    FOR EACH mark IN studentMarksList:
        IF mark >= threshold:
            passCount = passCount + 1
END
