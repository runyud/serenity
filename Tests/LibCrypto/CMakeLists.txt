set(TEST_SOURCES
    TestAES.cpp
    TestBigInteger.cpp
    TestChecksum.cpp
    TestChaCha20.cpp
    TestCurves.cpp
    TestHash.cpp
    TestHMAC.cpp
    TestPoly1305.cpp
    TestRSA.cpp
)

foreach(source IN LISTS TEST_SOURCES)
    serenity_test("${source}" LibCrypto LIBS LibCrypto)
endforeach()
