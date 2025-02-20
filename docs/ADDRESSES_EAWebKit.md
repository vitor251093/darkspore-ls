# Darkspore.exe EAWebKit Addresses
This is the list of known EAWebKit functions inside the Darkspore.exe. We are trying to find out how the game works to make the server, and for that, the more we know about the game code, the best.

## protossl.c
- **sub_E4B9E0:** `static int32_t _WildcardMatchNoCase(const char *pString1, const char *pString2)`
- **sub_E4BA60:** `static void _GenerateRandom(uint8_t *pRandomBuf, int32_t iRandomLen, CryptArc4T *pArc4)`
- **sub_E4BAD0:** ?
- **sub_E4BB30:** `static int32_t _ResetState(ProtoSSLRefT *pState, int32_t iSecure)`
- **sub_E4BC30:** `static int32_t _SendPacket(ProtoSSLRefT *pState, uint8_t uType, const void *pHeadPtr, int32_t iHeadLen, const void *pBodyPtr, int32_t iBodyLen)`
- **sub_E4BEF0:** `static int32_t _RecvPacket(ProtoSSLRefT *pState)`
- **sub_E4C2B0:** `static const void *_RecvHandshake(ProtoSSLRefT *pState, uint8_t uType)`
- **sub_E4C310:** `static const uint8_t *_FindPEMSignature(const uint8_t *pCertData, int32_t iCertSize, const char *pSigText)`
- **sub_E4C380:** `static int32_t _FindPEMCertificateData(const uint8_t *pCertData, int32_t iCertSize, const uint8_t **pCertBeg, const uint8_t **pCertEnd)`
- **sub_E4C410:** `static int32_t _CompareIdent(const ProtoSSLCertIdentT *pIdent1, const ProtoSSLCertIdentT *pIdent2)`
- **sub_E4C550:** `static const unsigned char *_ParseHeader(const unsigned char *pData, const unsigned char *pLast, int32_t *pType, int32_t *pSize)`
- **sub_E4C5C0:** ?
- **sub_E4C650:** `static int32_t _ParseCertificate(X509CertificateT *pCert, const uint8_t *pData, int32_t iSize)`
- **sub_E4D3F0:** ?
- **sub_E4D4D0:** `static int32_t _VerifyCertificate(X509CertificateT *pCert, int32_t iSelfSigned)`
- **sub_E4D570:** `static void _AddCertificate(X509CertificateT *pCert, int32_t iMemGroup, void *pMemGroupUserData)`
- **sub_E4D670:** `ProtoSSLRefT *ProtoSSLCreate(void)`
- **sub_E4D6D0:** ?
- **sub_E4D740:** `ProtoSSLRefT *ProtoSSLAccept(ProtoSSLRefT *pState, int32_t iSecure, struct sockaddr *pAddr, int32_t *pAddrlen)`
- **sub_E4D7C0:** ?
- **sub_E4D9A0:** ?
- **sub_E4DA00:** `static int32_t _ProtoSSLUpdateSendClientHello(ProtoSSLRefT *pState)`
- **sub_E4DAB0:** `static int32_t _ProtoSSLUpdateRecvServerHello(ProtoSSLRefT *pState, const uint8_t *pData)`
- **sub_E4DB30:** `static int32_t _ProtoSSLUpdateRecvServerCert(ProtoSSLRefT *pState, const uint8_t *pData)`
- **sub_E4DC00:** `static int32_t _ProtoSSLUpdateSendClientKey(ProtoSSLRefT *pState)`
- **sub_E4DEC0:** `static int32_t _ProtoSSLUpdateSendChange(ProtoSSLRefT *pState)`
- **sub_E4DF10:** `static int32_t _ProtoSSLUpdateSendClientFinish(ProtoSSLRefT *pState)`
- **sub_E4E0E0:** `static int32_t _ProtoSSLUpdateRecvChange(ProtoSSLRefT *pState, const uint8_t *pData)`
- **sub_E4E110:** `static int32_t _ProtoSSLUpdateRecvServerFinish(ProtoSSLRefT *pState, const uint8_t *pData)`
- **sub_E4E2F0:** `void ProtoSSLUpdate(ProtoSSLRefT *pState)`
- **sub_E4E720:** `int32_t ProtoSSLSend(ProtoSSLRefT *pState, const char *pBuffer, int32_t iLength)`
- **sub_E4E7B0:** `int32_t ProtoSSLRecv(ProtoSSLRefT *pState, char *pBuffer, int32_t iLength)`
- **sub_E4E8A0:** ?
- **sub_E4E9E0:** ?
- **sub_E4EA50:** `int32_t ProtoSSLSetCACert(const uint8_t *pCertData, int32_t iCertSize)`

- **sub_E4EC80:** ?
- **sub_E4ED30:** ?
- **sub_E4ED70:** ?
- **sub_E4ED90:** ?
- **sub_E4EE70:** ?
- **sub_E4EED0:** ?
- **sub_E4F100:** ?
- **sub_E4F1D0:** ?
- **sub_E4F260:** ?
- **sub_E4F2A0:** ?
- **sub_E4F310:** ?
- **sub_E4F410:** ?
- **sub_E4F470:** ?
- **sub_E4F5B0:** ?
- **sub_E4F6C0:** ?
- **sub_E4F6E0:** ?
- **sub_E4F700:** ?
- **sub_E4F7B0:** ?
- **sub_E4F860:** ?
- **sub_E4F890:** ?
- **sub_E4F9F0:** ?
- **sub_E4FA70:** ?
- **sub_E4FAE0:** ?
- **sub_E4FAF0:** ?
- **sub_E4FB70:** ?
- **sub_E4FCA0:** ?
- **sub_E4FCD0:** ?
- **sub_E4FCE0:** `DirtyMemGroupQuery`

- **sub_E4FFF0:** `NetTick`

### Socket
- **sub_E54160:** `SocketClose`
- **sub_E543A0:** `SocketAccept`
- **sub_E54400:** `SocketSend`

### cryptmd5.c
- **sub_E57310:** `CryptMD5Init`
- **sub_E57340:** `CryptMD5Update`
- **sub_E573F0:** `CryptMD5Final`

### cryptarc4.c
- **sub_E57D40:** `CryptArc4Init`
- **sub_E57DE0:** `CryptArc4Apply`

### cryptsha1.c
- **sub_E580A0:** `CryptSha1Init`
- **sub_E580E0:** `CryptSha1Update`
- **sub_E58190:** `CryptSha1Final`

### cryptrsa.c
- **sub_E58620:** `static void _Multiply(uint16_t *pResult, int32_t iWidth, uint16_t *pMul1, uint16_t *pMul2, uint16_t *pMod)`
- **sub_E58740:** `static int32_t _ToWords(uint16_t *pResult, int32_t iWidth, const uint8_t *pSource, int32_t iLength)`

- **sub_E587F0:** `static void _Exponentiate(uint8_t *pResult, uint8_t *pPowerof, const uint8_t *pModulus, int32_t iModSize,  const uint8_t *pExponent, int32_t iExpSize)`
- **sub_E58BA0:** `void CryptRSAInit(CryptRSAT *pState, const uint8_t *pModulus, int32_t iModSize, const uint8_t *pExponent, int32_t iExpSize)`
- **sub_E58C00:** `void CryptRSAInitMaster(CryptRSAT *pState, const uint8_t *pMaster, int32_t iMasterLen)`
- **sub_E58C80:** `void CryptRSAInitSignature(CryptRSAT *pState, const uint8_t *pSig, int32_t iSigLen)`
- **sub_E58C90:** `void CryptRSAEncrypt(CryptRSAT *pState)`

### lobbybase64.c
- **sub_E58CC0:** `LobbyBase64Decode`

## Important
If we can use Detours to modify `_ProtoSSLUpdateRecvServerCert`, in order to add `pState->bAllowAnyCert = true;` to the beginning of it, it will work without SSL.
