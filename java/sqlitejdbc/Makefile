PORTNAME=	sqlitejdbc
PORTVERSION=	056
DISTVERSIONPREFIX=	v
DISTVERSIONSUFFIX=	-src
PORTREVISION=	2
CATEGORIES=	java databases
MASTER_SITES=	http://files.zentus.com/sqlitejdbc/

MAINTAINER=	lapo@lapo.it
COMMENT=	Java JDBC driver for SQLite
WWW=		http://web.archive.org/web/20120721075310/http://www.zentus.com/sqlitejdbc/

LIB_DEPENDS=	libsqlite3.so:databases/sqlite3

USES=		gmake java tar:tgz
JAVA_VERSION=	8

WRKSRC=		${WRKDIR}/${PORTNAME}-${DISTVERSIONPREFIX}${DISTVERSION}
MAKE_ENV=	JAVA_HOME="${JAVA_HOME}"
ALL_TARGET=	native

PLIST_FILES=	${JAVAJARDIR}/sqlitejdbc-native.jar lib/libsqlitejdbc.so

do-install:
	${INSTALL_DATA} ${WRKSRC}/build/sqlitejdbc-v${PORTVERSION}-native.jar \
		${STAGEDIR}${JAVAJARDIR}/sqlitejdbc-native.jar
	${INSTALL_DATA} ${WRKSRC}/build/FreeBSD/libsqlitejdbc.so \
		${STAGEDIR}${PREFIX}/lib/

.include <bsd.port.mk>
