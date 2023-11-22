<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:amp="http://soprabanking.com/amplitude">
   <soapenv:Header/>
   <soapenv:Body>
      <amp:createTransferRequestFlow>
         <amp:requestHeader>
            <amp:requestId>1</amp:requestId>
            <amp:serviceName>createTransfer</amp:serviceName>
            <amp:timestamp>${=(new Date().format("yyyy-MM-dd'T'hh:mm:ss"))}</amp:timestamp>
            <amp:userCode>DAVID.ETE@</amp:userCode>
         </amp:requestHeader>
         <amp:createTransferRequest>
            <amp:canal>NEXTGEN</amp:canal>
            <amp:pain001><![CDATA[<?xml version='1.0' encoding='UTF-8'?>

<Document xmlns="urn:iso:std:iso:20022:tech:xsd:pain.001.001.03DB">
    <CstmrCdtTrfInitn>
        <GrpHdr>
            <MsgId>PERM_ANNUL_001</MsgId>
            <CreDtTm>${=(new Date().format("yyyy-MM-dd'T'hh:mm:ss"))}</CreDtTm>
            <NbOfTxs>1</NbOfTxs>
            <CtrlSum>45000</CtrlSum>
            <InitgPty/>
            <DltPrvtData>
                <FlwInd>HOMOLOGATION</FlwInd>
                <DltPrvtDataDtl>
                    <PrvtDtInf>NEXTGEN</PrvtDtInf>
                    <Tp>
                        <CdOrPrtry>
                            <Cd>CHANNEL</Cd>
                        </CdOrPrtry>
                    </Tp>
                </DltPrvtDataDtl>
            </DltPrvtData>
        </GrpHdr>
        <PmtInf>
            <PmtInfId>PERM_ANNUL_001</PmtInfId>
            <PmtMtd>TRF</PmtMtd>
            <BtchBookg>false</BtchBookg>
            <NbOfTxs>1</NbOfTxs>
            <CtrlSum>45000</CtrlSum>
			
			<DltPrvtData>
				<OrdrPrties>
				  <Tp>STO</Tp>
				  <Md>CREATE</Md>
				  <StdgOrdrInf>
					<Frqcy>MNTH</Frqcy>
					<NbOfInstlments>4</NbOfInstlments>
					<FrstInstlmentDt>2023-03-24</FrstInstlmentDt>
					<LstInstlmentDt>2023-06-24</LstInstlmentDt>
				  </StdgOrdrInf>
				</OrdrPrties>
			 </DltPrvtData>
			
            <PmtTpInf>
                <InstrPrty>NORM</InstrPrty>
                <SvcLvl>
                    <Prtry>INTERNAL</Prtry>
                </SvcLvl>
            </PmtTpInf>
            <ReqdExctnDt>2023-03-23</ReqdExctnDt>
            <Dbtr>
                <Nm>NOM DONNEUR D'ORDRE</Nm>
            </Dbtr>
            <DbtrAcct>
                <Id>
                    <Othr>
                        <Id>111049153</Id>
                        <SchmeNm>
                            <Prtry>BKCOM_ACCOUNT</Prtry>
                        </SchmeNm>
                    </Othr>
                </Id>
                <Ccy>XOF</Ccy>
            </DbtrAcct>
            <DbtrAgt>
                <FinInstnId>
                    <Nm>BANQUE SGCI</Nm>
                    <Othr>
                        <Id>CI008</Id>
                        <SchmeNm>
                            <Prtry>ITF_DELTAMOP_IDETAB</Prtry>
                        </SchmeNm>
                    </Othr>
                </FinInstnId>
                <BrnchId>
                    <Id>00111</Id>
                    <Nm>AGENCE CITE CHEMIN DE FER</Nm>
                </BrnchId>
            </DbtrAgt>
            <ChrgBr>SHAR</ChrgBr>
            
            
            <CdtTrfTxInf>
                <PmtId>
                    <InstrId>PERM_ANNUL_001</InstrId>
                    <EndToEndId>PERM_ANNUL_001</EndToEndId>
                </PmtId>
                <Amt>
                    <InstdAmt Ccy="XOF">45000</InstdAmt>
                </Amt>
                <CdtrAgt>
                    <FinInstnId>
                        <Nm>BANQUE SGG</Nm>
                        <Othr>
                            <Id>CI008</Id>
                            <SchmeNm>
                                <Prtry>ITF_DELTAMOP_IDETAB</Prtry>
                            </SchmeNm>
                        </Othr>
                    </FinInstnId>
                    <BrnchId>
                        <Id>00110</Id>
                        <Nm>AGENCE KAMSAR</Nm>
                    </BrnchId>
                </CdtrAgt>
                <Cdtr>
                    <Nm>NOM DU BENEFICIAIRE</Nm>
                </Cdtr>
                <CdtrAcct>
                    <Id>
                        <Othr>
                            <Id>110400015</Id>
                            <SchmeNm>
                                <Prtry>BKCOM_ACCOUNT</Prtry>
                            </SchmeNm>
                        </Othr>
                    </Id>
                    <Ccy>XOF</Ccy>
                </CdtrAcct>
                <RmtInf>
                    <Ustrd>Virement Dom NEXTGEN</Ustrd>
                </RmtInf>
            </CdtTrfTxInf>
        </PmtInf>
    </CstmrCdtTrfInitn>
</Document>]]></amp:pain001>
         </amp:createTransferRequest>
      </amp:createTransferRequestFlow>
   </soapenv:Body>
</soapenv:Envelope>
