	
BEGIN

    SET threshold ← 50
    SET passCount ← 0

    INPUT studentMarksList
    SET totalStudents ← LENGTH (studentMarksList)

    FOR EACH mark IN studentMarksList DO
        IF mark ≥ threshold THEN
            passCount ← passCount + 1
        ELSE
            passCount ← passCount + 0
        END IF
    END FOR

    IF passCount ≥ (totalStudents / 2) THEN
        OUTPUT "Module Performance: Strength"
    ELSE
        OUTPUT "Module Performance: Weak Area"
    END IF

END
